<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2.0.0-rc.3`](#caddy200-rc3)
-	[`caddy:2.0.0-rc.3-alpine`](#caddy200-rc3-alpine)
-	[`caddy:2.0.0-rc.3-builder`](#caddy200-rc3-builder)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:latest`](#caddylatest)

## `caddy:2.0.0-rc.3`

```console
$ docker pull caddy@sha256:e971c7f178f63f7c33652f03cf6aaa12da99dfbab95ae3352184f31808c5b2b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `caddy:2.0.0-rc.3` - linux; amd64

```console
$ docker pull caddy@sha256:555b7bca74bab92cf1c1ee8d7f6bbe2ea7e6740e74d16eb83d1ee88e0e45da65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27077360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4dd95cbddf7112ba81aecb08b1cb581e5732dc9c9bdae157243d51db121725`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 13 Apr 2020 23:43:04 GMT
RUN apk add --no-cache ca-certificates
# Mon, 13 Apr 2020 23:43:04 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 13 Apr 2020 23:43:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_CHECKSUM_SHA512=32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88
# Mon, 13 Apr 2020 23:43:11 GMT
RUN set -eux; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_amd64.tar.gz"; 	echo "$CADDY_CHECKSUM_SHA512  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 13 Apr 2020 23:43:11 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 13 Apr 2020 23:43:11 GMT
ENV XDG_DATA_HOME=/data
# Mon, 13 Apr 2020 23:43:12 GMT
VOLUME [/config]
# Mon, 13 Apr 2020 23:43:12 GMT
VOLUME [/data]
# Mon, 13 Apr 2020 23:43:12 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 13 Apr 2020 23:43:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 13 Apr 2020 23:43:15 GMT
EXPOSE 80
# Mon, 13 Apr 2020 23:43:15 GMT
EXPOSE 443
# Mon, 13 Apr 2020 23:43:16 GMT
EXPOSE 2019
# Mon, 13 Apr 2020 23:43:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34768c0e097ae8d61b298bc7f4f92fb388c048edba171f5b0ce6b43529fe44c`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 301.3 KB (301287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8542e370608b22a8c405d41ba15bb6318bb044928e806a24084eb77593ecac`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87232ade1118b56aa98b50924838ab5654b59e3a231c2a8ee9056ac0530c873`  
		Last Modified: Mon, 13 Apr 2020 23:44:19 GMT  
		Size: 24.0 MB (23967051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-rc.3-alpine`

```console
$ docker pull caddy@sha256:e971c7f178f63f7c33652f03cf6aaa12da99dfbab95ae3352184f31808c5b2b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `caddy:2.0.0-rc.3-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:555b7bca74bab92cf1c1ee8d7f6bbe2ea7e6740e74d16eb83d1ee88e0e45da65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27077360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4dd95cbddf7112ba81aecb08b1cb581e5732dc9c9bdae157243d51db121725`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 13 Apr 2020 23:43:04 GMT
RUN apk add --no-cache ca-certificates
# Mon, 13 Apr 2020 23:43:04 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 13 Apr 2020 23:43:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_CHECKSUM_SHA512=32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88
# Mon, 13 Apr 2020 23:43:11 GMT
RUN set -eux; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_amd64.tar.gz"; 	echo "$CADDY_CHECKSUM_SHA512  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 13 Apr 2020 23:43:11 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 13 Apr 2020 23:43:11 GMT
ENV XDG_DATA_HOME=/data
# Mon, 13 Apr 2020 23:43:12 GMT
VOLUME [/config]
# Mon, 13 Apr 2020 23:43:12 GMT
VOLUME [/data]
# Mon, 13 Apr 2020 23:43:12 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 13 Apr 2020 23:43:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 13 Apr 2020 23:43:15 GMT
EXPOSE 80
# Mon, 13 Apr 2020 23:43:15 GMT
EXPOSE 443
# Mon, 13 Apr 2020 23:43:16 GMT
EXPOSE 2019
# Mon, 13 Apr 2020 23:43:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34768c0e097ae8d61b298bc7f4f92fb388c048edba171f5b0ce6b43529fe44c`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 301.3 KB (301287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8542e370608b22a8c405d41ba15bb6318bb044928e806a24084eb77593ecac`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87232ade1118b56aa98b50924838ab5654b59e3a231c2a8ee9056ac0530c873`  
		Last Modified: Mon, 13 Apr 2020 23:44:19 GMT  
		Size: 24.0 MB (23967051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-rc.3-builder`

```console
$ docker pull caddy@sha256:d1a2e2a7be73ebbd649b0e0e70e5fbef495135ba8994b12398b9cb57443f64f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `caddy:2.0.0-rc.3-builder` - linux; amd64

```console
$ docker pull caddy@sha256:486d86fe70265203228afb9b9e6e7934019090c6686da9a9fb98579931a05778
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322863984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fd06ca5bdeb1a36375ba63a93a06401045ebb7a6154830e973a6de5949242b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:02:02 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 23:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:06:10 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:11:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:11:13 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:11:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:11:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:11:16 GMT
WORKDIR /go
# Mon, 13 Apr 2020 23:43:21 GMT
WORKDIR /src
# Mon, 13 Apr 2020 23:43:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 13 Apr 2020 23:43:24 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:27 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 13 Apr 2020 23:43:27 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 13 Apr 2020 23:43:57 GMT
RUN go get -d ./...
# Mon, 13 Apr 2020 23:43:59 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 13 Apr 2020 23:43:59 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c732a2540651eb09faab95b03b3b5928ab23e096fae0006bdc2abf9e0cb5bfb4`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 301.3 KB (301283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2225181d6bcfb7877529a7257ff207cb14e52831420f770cbc2187031b6228`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdfa13e5b48c976ba308826b27a4978c2ffe6833efcfcfc0bd40dbf25e88455`  
		Last Modified: Wed, 08 Apr 2020 23:26:23 GMT  
		Size: 132.0 MB (132012220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c48a539365d2d572e18de4a42ab11b02d9870a17bf1f65160d7fcbbd0423263`  
		Last Modified: Wed, 08 Apr 2020 23:25:47 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947fdad36c6d1e2fd7b618aa1a49dfabaa1ff9d6fb85a195e2437c2b9ac78142`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199e6b2236a218d72efd03fc1fa0971c00c87439722e1a40269b7edfd910b79`  
		Last Modified: Mon, 13 Apr 2020 23:44:28 GMT  
		Size: 8.2 MB (8155831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732862f7439776bbe7cc313ed1e10454506f168429234c0daea17d6c48a9692`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 2.7 MB (2744273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54fb1573600e831b250c83cb9dc699bab8aa12040568d9ee542fb8d09c1d99`  
		Last Modified: Mon, 13 Apr 2020 23:45:02 GMT  
		Size: 176.8 MB (176846093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e336ec02e20348f57d1ef8151ecfcd216777f5489f01b29164883ec496bcbb`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6f8a2da1c847ae8cd10d1f3e37ad75cc0ba17c5e9b4f7e68fdd3b7cffb5482`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:e971c7f178f63f7c33652f03cf6aaa12da99dfbab95ae3352184f31808c5b2b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `caddy:alpine` - linux; amd64

```console
$ docker pull caddy@sha256:555b7bca74bab92cf1c1ee8d7f6bbe2ea7e6740e74d16eb83d1ee88e0e45da65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27077360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4dd95cbddf7112ba81aecb08b1cb581e5732dc9c9bdae157243d51db121725`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 13 Apr 2020 23:43:04 GMT
RUN apk add --no-cache ca-certificates
# Mon, 13 Apr 2020 23:43:04 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 13 Apr 2020 23:43:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_CHECKSUM_SHA512=32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88
# Mon, 13 Apr 2020 23:43:11 GMT
RUN set -eux; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_amd64.tar.gz"; 	echo "$CADDY_CHECKSUM_SHA512  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 13 Apr 2020 23:43:11 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 13 Apr 2020 23:43:11 GMT
ENV XDG_DATA_HOME=/data
# Mon, 13 Apr 2020 23:43:12 GMT
VOLUME [/config]
# Mon, 13 Apr 2020 23:43:12 GMT
VOLUME [/data]
# Mon, 13 Apr 2020 23:43:12 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 13 Apr 2020 23:43:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 13 Apr 2020 23:43:15 GMT
EXPOSE 80
# Mon, 13 Apr 2020 23:43:15 GMT
EXPOSE 443
# Mon, 13 Apr 2020 23:43:16 GMT
EXPOSE 2019
# Mon, 13 Apr 2020 23:43:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34768c0e097ae8d61b298bc7f4f92fb388c048edba171f5b0ce6b43529fe44c`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 301.3 KB (301287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8542e370608b22a8c405d41ba15bb6318bb044928e806a24084eb77593ecac`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87232ade1118b56aa98b50924838ab5654b59e3a231c2a8ee9056ac0530c873`  
		Last Modified: Mon, 13 Apr 2020 23:44:19 GMT  
		Size: 24.0 MB (23967051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:d1a2e2a7be73ebbd649b0e0e70e5fbef495135ba8994b12398b9cb57443f64f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:486d86fe70265203228afb9b9e6e7934019090c6686da9a9fb98579931a05778
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322863984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fd06ca5bdeb1a36375ba63a93a06401045ebb7a6154830e973a6de5949242b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:02:02 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 23 Mar 2020 23:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Apr 2020 23:06:10 GMT
ENV GOLANG_VERSION=1.14.2
# Wed, 08 Apr 2020 23:11:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '98de84e69726a66da7b4e58eac41b99cbe274d7e8906eeb8a5b7eb0aadee7f7c *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Wed, 08 Apr 2020 23:11:13 GMT
ENV GOPATH=/go
# Wed, 08 Apr 2020 23:11:14 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Apr 2020 23:11:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 08 Apr 2020 23:11:16 GMT
WORKDIR /go
# Mon, 13 Apr 2020 23:43:21 GMT
WORKDIR /src
# Mon, 13 Apr 2020 23:43:23 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 13 Apr 2020 23:43:24 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:27 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 13 Apr 2020 23:43:27 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 13 Apr 2020 23:43:57 GMT
RUN go get -d ./...
# Mon, 13 Apr 2020 23:43:59 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 13 Apr 2020 23:43:59 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c732a2540651eb09faab95b03b3b5928ab23e096fae0006bdc2abf9e0cb5bfb4`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 301.3 KB (301283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2225181d6bcfb7877529a7257ff207cb14e52831420f770cbc2187031b6228`  
		Last Modified: Mon, 23 Mar 2020 23:13:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdfa13e5b48c976ba308826b27a4978c2ffe6833efcfcfc0bd40dbf25e88455`  
		Last Modified: Wed, 08 Apr 2020 23:26:23 GMT  
		Size: 132.0 MB (132012220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c48a539365d2d572e18de4a42ab11b02d9870a17bf1f65160d7fcbbd0423263`  
		Last Modified: Wed, 08 Apr 2020 23:25:47 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947fdad36c6d1e2fd7b618aa1a49dfabaa1ff9d6fb85a195e2437c2b9ac78142`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199e6b2236a218d72efd03fc1fa0971c00c87439722e1a40269b7edfd910b79`  
		Last Modified: Mon, 13 Apr 2020 23:44:28 GMT  
		Size: 8.2 MB (8155831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732862f7439776bbe7cc313ed1e10454506f168429234c0daea17d6c48a9692`  
		Last Modified: Mon, 13 Apr 2020 23:44:26 GMT  
		Size: 2.7 MB (2744273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54fb1573600e831b250c83cb9dc699bab8aa12040568d9ee542fb8d09c1d99`  
		Last Modified: Mon, 13 Apr 2020 23:45:02 GMT  
		Size: 176.8 MB (176846093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e336ec02e20348f57d1ef8151ecfcd216777f5489f01b29164883ec496bcbb`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6f8a2da1c847ae8cd10d1f3e37ad75cc0ba17c5e9b4f7e68fdd3b7cffb5482`  
		Last Modified: Mon, 13 Apr 2020 23:44:25 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:e971c7f178f63f7c33652f03cf6aaa12da99dfbab95ae3352184f31808c5b2b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:555b7bca74bab92cf1c1ee8d7f6bbe2ea7e6740e74d16eb83d1ee88e0e45da65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27077360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4dd95cbddf7112ba81aecb08b1cb581e5732dc9c9bdae157243d51db121725`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 13 Apr 2020 23:43:04 GMT
RUN apk add --no-cache ca-certificates
# Mon, 13 Apr 2020 23:43:04 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 13 Apr 2020 23:43:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_VERSION=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:07 GMT
ENV CADDY_CHECKSUM_SHA512=32735a963f946bf561ed2a540192c22ad19565be4bce4bc243c61beae9022ca15a54bf5ef8a5f2341bd3af16fd7b0e9f7832697687201a981a2ac52b0c18ca88
# Mon, 13 Apr 2020 23:43:11 GMT
RUN set -eux; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0-rc.3/caddy_2.0.0-rc.3_linux_amd64.tar.gz"; 	echo "$CADDY_CHECKSUM_SHA512  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 13 Apr 2020 23:43:11 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 13 Apr 2020 23:43:11 GMT
ENV XDG_DATA_HOME=/data
# Mon, 13 Apr 2020 23:43:12 GMT
VOLUME [/config]
# Mon, 13 Apr 2020 23:43:12 GMT
VOLUME [/data]
# Mon, 13 Apr 2020 23:43:12 GMT
LABEL org.opencontainers.image.version=v2.0.0-rc.3
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 13 Apr 2020 23:43:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 13 Apr 2020 23:43:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 13 Apr 2020 23:43:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 13 Apr 2020 23:43:15 GMT
EXPOSE 80
# Mon, 13 Apr 2020 23:43:15 GMT
EXPOSE 443
# Mon, 13 Apr 2020 23:43:16 GMT
EXPOSE 2019
# Mon, 13 Apr 2020 23:43:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34768c0e097ae8d61b298bc7f4f92fb388c048edba171f5b0ce6b43529fe44c`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 301.3 KB (301287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8542e370608b22a8c405d41ba15bb6318bb044928e806a24084eb77593ecac`  
		Last Modified: Mon, 13 Apr 2020 23:44:13 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87232ade1118b56aa98b50924838ab5654b59e3a231c2a8ee9056ac0530c873`  
		Last Modified: Mon, 13 Apr 2020 23:44:19 GMT  
		Size: 24.0 MB (23967051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
