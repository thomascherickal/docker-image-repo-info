## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:9f2442e39180a6b96658075c5ff728c664269c7bbfc27b27d937ec4acdb5d6bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:314c50c29850a72f3fd99e9d343941c604d9c1ba44e9847952dbe1d3ebe9dc00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119494851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0082606d369ae992d43cc62883c46f0d3edbd2f405f2921be3df2a45c97e1`
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
# Fri, 05 Feb 2021 03:31:04 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 03:35:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 03:35:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 03:35:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 03:35:48 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 03:35:48 GMT
WORKDIR /go
# Fri, 05 Feb 2021 05:35:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 05:35:13 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 05:35:24 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 05:35:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 05:35:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 05:35:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 05:35:26 GMT
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
	-	`sha256:92c4e5d29c8852785ed5720528a00d03c8fc8ad36291f155dc43ecb0c49a7fbc`  
		Last Modified: Fri, 05 Feb 2021 03:47:26 GMT  
		Size: 106.8 MB (106795928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf68fc69aa551ba07d298a123308c2ceee7d19e46b497165fd24be462dea8890`  
		Last Modified: Fri, 05 Feb 2021 03:47:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae6c005f9632a0e0b4189898352004d5e756d63c574fc99f1174b5f65d5a98`  
		Last Modified: Fri, 05 Feb 2021 05:35:53 GMT  
		Size: 8.3 MB (8310006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e247dc23f67335195c98d2ecdce71b595043e974c4df36ae394d7e11ff2165`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 1.3 MB (1308354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1999deb1377f933660819664539f19e5bd83c9c3151c70ac8cbd3c7f0bf1b3`  
		Last Modified: Fri, 05 Feb 2021 05:35:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

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

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fdcaf52c0076b069aa85685e3fe6a20697d8b70438b8dd821e9ac8feb72a1777
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113509014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050f039cff2bdd8abe348599ca0fd389cc0f605742af2abd34222667898ee73e`
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
# Fri, 05 Feb 2021 02:35:56 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:38:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:38:46 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:38:50 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:38:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:38:54 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:09:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:09:24 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:09:40 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:09:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:09:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:09:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:09:45 GMT
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
	-	`sha256:69b997820a9ac5f4fbb29e18254c1b2c7530aceda5e4f94c207d2ddd2d51bcde`  
		Last Modified: Fri, 05 Feb 2021 02:52:36 GMT  
		Size: 102.5 MB (102458602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09f519e526d0b1bf0c7e6caeff1aa92724e67c8a6a5054f82f1526f2956ba6`  
		Last Modified: Fri, 05 Feb 2021 02:52:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d1870c10190ab40e93935a8c269d95e2e9b78384159c24ed02e0f2c80b86e`  
		Last Modified: Fri, 05 Feb 2021 04:10:12 GMT  
		Size: 7.1 MB (7145159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff5f06fe9e54733fbda02a77a0cddca938b3e2f5ab8fd317c93430d6cda5a86`  
		Last Modified: Fri, 05 Feb 2021 04:10:19 GMT  
		Size: 1.2 MB (1216924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2ec272a20020ac41b27a756c91c7572a3cfbdc0f4489fec0b76de27248812f`  
		Last Modified: Fri, 05 Feb 2021 04:10:18 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e1f434fd2084f25a078fe6d7428c322ae1fa67e229dfc3338b088f67e52f45da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114818485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ec43dd925d96811bc9265cd951a348272d90f517e93fde6ea811ede3e1d92`
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
# Fri, 05 Feb 2021 02:18:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 02:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 02:20:14 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 02:20:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 02:20:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 02:20:18 GMT
WORKDIR /go
# Fri, 05 Feb 2021 04:00:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 04:00:57 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 04:01:21 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 04:01:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 04:01:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 04:01:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 04:01:26 GMT
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
	-	`sha256:badb0947eceb8c60e51fae1a104dd1e5d5523a9d911ff6ce46e67561137829d2`  
		Last Modified: Fri, 05 Feb 2021 02:32:16 GMT  
		Size: 102.1 MB (102128074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202117b65d73f7da5b89d040b78a12d631164b0d7040bcaba871e53b8b3ad9d`  
		Last Modified: Fri, 05 Feb 2021 02:31:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c047bbe2ae81d95b0fa8b3f76afde945d75faf5f7bfc3df7ae6298e5c48d7b1`  
		Last Modified: Fri, 05 Feb 2021 04:01:53 GMT  
		Size: 8.5 MB (8499908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b81bb2919f0b02b482dcff56569bcce6e633646a952ee9e9902c8f0d72838b4`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 1.2 MB (1199526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b59ccfb95698d2b5afa42795ad4b47e22199f83010272837664c394092d9b6`  
		Last Modified: Fri, 05 Feb 2021 04:02:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f995aef3894dabac8bffee8e8ef0ce3441c554b467ff764887060bf1debc8ec7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113974061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041b89b17caff67e2ff11c1f841db87e9beceae6e39da54610e60c29c4708aaa`
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
# Fri, 05 Feb 2021 08:52:11 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:54:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:54:38 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:54:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:55:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:55:07 GMT
WORKDIR /go
# Fri, 05 Feb 2021 12:03:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 12:03:44 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 12:04:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 12:05:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 12:05:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 12:05:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 12:05:23 GMT
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
	-	`sha256:a16885882ebdf3e195f9b28193040774d1c56efa0f5f0ecf8de40294cbc90f59`  
		Last Modified: Fri, 05 Feb 2021 09:17:03 GMT  
		Size: 100.8 MB (100795887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3be9eef8b0872834da5b1f172fdca0895dbcc35812979dfd33ee559060502c`  
		Last Modified: Fri, 05 Feb 2021 09:16:40 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fa5ff36055008e584e081ef157b4063c4d8e30fdb6d2aa34b05643dac08114`  
		Last Modified: Fri, 05 Feb 2021 12:05:53 GMT  
		Size: 8.9 MB (8920048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddde52fc52e8ace8684032b68c6980757fe3d2a177218b8dfadf9fbbb517f2`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 1.2 MB (1168985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9ed4317206a38a1788ac8bad02a5dc7bdbc4c749b5b328e8399113da143ffe`  
		Last Modified: Fri, 05 Feb 2021 12:06:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0374b2cd79d1180c346ad765ae1ca6d1e3c461c74820940268b860b6015ac2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118372183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48df5f2b0f642b42b13681a61493b468491737a5085815d7ca05ec801473c4bb`
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
# Fri, 05 Feb 2021 08:27:15 GMT
ENV GOLANG_VERSION=1.15.8
# Fri, 05 Feb 2021 08:31:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.15.8.src.tar.gz'; 	sha256='540c0ab7781084d124991321ed1458e479982de94454a98afab6acadf38497c2'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 05 Feb 2021 08:31:23 GMT
ENV GOPATH=/go
# Fri, 05 Feb 2021 08:31:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 05 Feb 2021 08:31:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 05 Feb 2021 08:31:26 GMT
WORKDIR /go
# Fri, 05 Feb 2021 11:44:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 05 Feb 2021 11:44:54 GMT
ENV XCADDY_VERSION=v0.1.7
# Fri, 05 Feb 2021 11:45:08 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 05 Feb 2021 11:45:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 05 Feb 2021 11:45:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='5528906e2cbaad7c5fa94ed7c00c12c97b2df67aac58a4fcb56e81d6378cfe9966e3975ac7976c7a508bdf5ee3cb3670666802dea21ee422461f563c7eb15229' ;; 		armhf)   binArch='armv6'; checksum='86825b4d1d9f50808f9a902a6697c038c8fb995f1d3f187607afcc85a7cd7cb0ef69f9d37c1a3543a618aea7ed07eca01188aa80861e2e336b6b4c44ea66e325' ;; 		armv7)   binArch='armv7'; checksum='bee5ef9dd43914f4b859d8c8f926692332d9d7d7bd59e1490c156d89109912a992b287f53014727b422bfcd26b052a561b695da15786fb218174393a32d55ca0' ;; 		aarch64) binArch='arm64'; checksum='0b846ce4d43dbaefc5b2e34acf33406454195bc1ac2ff51af0864a7755206d9c0e712e05b5519ad0fb194a0461790e3dafb3d11adc7572a4bb9035fc377aee66' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='330d806c656738a6f5e68a813cbcdf1065e6918b77985de0a8e3e5fa2a0a8c4c4fc17b7e115ad9a96707158a49cd3907c805efb61af41755ccc5f8dba3a2020e' ;; 		s390x)   binArch='s390x'; checksum='fbadef6768b8f3db17a66bc1ff114203c9acf559ebc8163bed4a983e4fb778d40e81f4f06a917a527de62220474400165886e143e5e5de1287239bebc1d026ba' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.7/xcaddy_0.1.7_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 05 Feb 2021 11:45:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 05 Feb 2021 11:45:11 GMT
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
	-	`sha256:4160a7b3a89e5333017c849993b4e19d68bbb2bf993b2fc6142c73e8d23ae65b`  
		Last Modified: Fri, 05 Feb 2021 08:48:21 GMT  
		Size: 105.9 MB (105908164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fb3687fd88203dd52d10eec02bd0093a66774458e2c700349dde892e193047`  
		Last Modified: Fri, 05 Feb 2021 08:48:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875cb511518c9503e34a4ffe365ee7a60017cb13512fef77a9b5e7029b8dea60`  
		Last Modified: Fri, 05 Feb 2021 11:46:13 GMT  
		Size: 8.4 MB (8352284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db0f7b6cd3bc8b63a9875c7a3eca56df42077937ff18e5a5aed5c9b6cc845`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 1.3 MB (1262676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7af1563d0813e5cfddc05a18e44941c4a97010fcf82244f842f17f9a2321b`  
		Last Modified: Fri, 05 Feb 2021 11:47:15 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
