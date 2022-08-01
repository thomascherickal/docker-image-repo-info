## `caddy:alpine`

```console
$ docker pull caddy@sha256:a4efe45e04bf5c1e057b81f79e22e9ed15662e78101bf179362f7589903f2cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:alpine` - linux; amd64

```console
$ docker pull caddy@sha256:2728a7a5cc9045d475a134f9230565677fe26deb5306060a0ab766d8449f6ba4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d954b31fe122c95e58bd7257e100408c9a17c064b065f4c723b46640b61d150c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:21:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 19 Jul 2022 00:21:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 19 Jul 2022 00:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 19 Jul 2022 00:21:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 80
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 443
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 2019
# Tue, 19 Jul 2022 00:21:09 GMT
WORKDIR /srv
# Tue, 19 Jul 2022 00:21:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0a25d662370cef41a6edf3bceddbd2bda0675eb94f8568d038b7356230396`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 291.6 KB (291612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a501877fabbb599942a33a45603240e372d191f8322b000c5aafec5a5090c4e`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c62335257e66d56f8fe9203793fb935200c4788ae2328fc7820374794f3d56`  
		Last Modified: Tue, 19 Jul 2022 00:21:36 GMT  
		Size: 13.9 MB (13916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4608ab095ff261532ff3818afb28725d2548a4d242c96ba13bd0e268249e6a`  
		Last Modified: Tue, 19 Jul 2022 00:21:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a4faffc4f2a46ebc00ece376d805f6be85e994de0d8d98175f84c9ab7e568ee0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16281124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f6682a24f2943790bb0fa25e153cbf1e6b2710c492901e466766ee30b8107d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 01 Aug 2022 17:53:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 01 Aug 2022 17:53:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 01 Aug 2022 17:53:17 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:53:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 01 Aug 2022 17:53:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 01 Aug 2022 17:53:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 01 Aug 2022 17:53:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 01 Aug 2022 17:53:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 80
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 443
# Mon, 01 Aug 2022 17:53:21 GMT
EXPOSE 2019
# Mon, 01 Aug 2022 17:53:21 GMT
WORKDIR /srv
# Mon, 01 Aug 2022 17:53:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf198df6d3b9a14a8c1f9d5cff7ff7e837de2bf2fda4e86bc7ad4162f7bf558`  
		Last Modified: Mon, 01 Aug 2022 17:54:07 GMT  
		Size: 304.5 KB (304528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58eb272d93ebe45b0a46f034b4330a4ede9d459fc6770dfa28bc676000379e`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 5.8 KB (5834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cce94f3d2ebd2f4f137aef8435742860d4af63c0f7ef8b7895f74526230be2`  
		Last Modified: Mon, 01 Aug 2022 17:54:09 GMT  
		Size: 13.4 MB (13364178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce8d08db4149d1084772ab0eae3b77b4e98b15ae51c7b7d9269bd2646a4717`  
		Last Modified: Mon, 01 Aug 2022 17:54:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5f08857dd953ec255ac0730fe3386348d3c05794c15932feed11965113e0032e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c821db573afbe6b3c70d1316bb06ac6b8f9dd3e611d8334b5b9ec57767be965c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Sat, 30 Jul 2022 11:42:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 30 Jul 2022 11:42:45 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Sat, 30 Jul 2022 11:42:45 GMT
ENV CADDY_VERSION=v2.5.2
# Sat, 30 Jul 2022 11:42:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 30 Jul 2022 11:42:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 30 Jul 2022 11:42:48 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 30 Jul 2022 11:42:48 GMT
ENV XDG_DATA_HOME=/data
# Sat, 30 Jul 2022 11:42:48 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Sat, 30 Jul 2022 11:42:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 30 Jul 2022 11:42:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 30 Jul 2022 11:42:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 30 Jul 2022 11:42:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 30 Jul 2022 11:42:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 30 Jul 2022 11:42:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 30 Jul 2022 11:42:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 30 Jul 2022 11:42:49 GMT
EXPOSE 80
# Sat, 30 Jul 2022 11:42:49 GMT
EXPOSE 443
# Sat, 30 Jul 2022 11:42:49 GMT
EXPOSE 2019
# Sat, 30 Jul 2022 11:42:49 GMT
WORKDIR /srv
# Sat, 30 Jul 2022 11:42:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272c2d250632d11188bdec6445f20055480bd7781bb36eb0c083be90047d1a8`  
		Last Modified: Sat, 30 Jul 2022 11:43:33 GMT  
		Size: 290.8 KB (290770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0938958a9d07aa6a5839788ab8c3159dc44e9ca6cb0581090f0bad58fc24f503`  
		Last Modified: Sat, 30 Jul 2022 11:43:33 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29b2e6f2d0e9b49bcbb96b258d0a842325c4294d63e67b3b6f2ef030164ba71`  
		Last Modified: Sat, 30 Jul 2022 11:43:36 GMT  
		Size: 13.3 MB (13347759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe76ed77ff0c1e94ca67a9fae25fbb431ca0d058d0f8c9f0d1934aceb44cb01c`  
		Last Modified: Sat, 30 Jul 2022 11:43:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7542ee62db8e10442071d4e9745bcd98f39619bcf9f516c1c9b4ecfc5cc0f3d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15721249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db56606eb0d00c279248ae38995824f79f994477565532beb03699a02e7f94af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:18:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:18:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:18:33 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:18:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:18:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:18:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:18:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:18:39 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:18:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:18:47 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:18:48 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:18:49 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:18:50 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:18:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6867c1bed7442ba6f8c33877f0a64552b8eb6e640825b2b39521a3ee4d3b7`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 291.5 KB (291464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9d0dc3dac6c9ea9c214169993cbf654f21972b33784651a2e35c75b2c3332`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818fab46ac8ba80668e14951d7ac785048f4df50fda97f61507062a61e3b1ad`  
		Last Modified: Mon, 18 Jul 2022 22:19:28 GMT  
		Size: 12.7 MB (12729160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef202eac441dd743baac9767af96c921d6a74c7b67ddb0da6989963669cc967`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d4ed904cc09a91c433a9ef0c27b7daad6550e02f6a4ec80f2bcc2b5bfb011d64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf5a90d8199b6618c768f8040a3f1cdb2a154789fa6612c7f6daf9362344d62`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Jul 2022 09:29:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 28 Jul 2022 09:29:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 28 Jul 2022 09:29:17 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Jul 2022 09:29:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Jul 2022 09:29:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 80
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 443
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 2019
# Thu, 28 Jul 2022 09:29:26 GMT
WORKDIR /srv
# Thu, 28 Jul 2022 09:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143cf45bb3764aa69910cc3bf88d9796600ad505fe7af4d3c67695d3531cea7b`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 294.0 KB (293972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97069a68d5f45ed80b3cf6952f9b94df5d5b2010f5ba70d24213b45cc2f7477`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee64bce4f5dd3491e75b5b2531cef2c68bc6cf0923aed600cf5b2c6549fa56ba`  
		Last Modified: Thu, 28 Jul 2022 09:30:15 GMT  
		Size: 12.3 MB (12309528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec473101201222cbe558f78a93799ab07b4b225382711f56d995cfb848bf5c6`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:28adfc1e1d82c412767e4b170580d554b8dbb36c1cb5b355005e2dc8c2eeb0b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a387c6224fd249160f6c2f8ffd24f60c57c927a1a599ce91609c9c27288434c7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:02:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 21:02:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 21:02:25 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 21:02:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 21:02:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 21:02:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 21:02:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 21:02:38 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 21:02:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 21:02:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 21:02:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 21:02:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 21:02:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 80
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 443
# Mon, 18 Jul 2022 21:02:46 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 21:02:46 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 21:02:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01286e5b65105b357bf83e8daa3cbc0a1a069a4d14af918fcd5475246f6af1b`  
		Last Modified: Mon, 18 Jul 2022 21:03:38 GMT  
		Size: 291.9 KB (291948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ce119bc29da400dd00bd331789e14fab9587661da4bb3e57835053afeb50b7`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8470e2e663127d3838fb96d9115f33c868c378cea548725085b75d9f39599548`  
		Last Modified: Mon, 18 Jul 2022 21:03:40 GMT  
		Size: 13.5 MB (13460687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e115a0286c47b77821e5d98da581e1d3e1f85b3dd134111f6c27790d0c45fbae`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
