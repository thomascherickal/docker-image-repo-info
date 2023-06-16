<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:1.5.9`](#kapacitor159)
-	[`kapacitor:1.5.9-alpine`](#kapacitor159-alpine)
-	[`kapacitor:1.6`](#kapacitor16)
-	[`kapacitor:1.6-alpine`](#kapacitor16-alpine)
-	[`kapacitor:1.6.6`](#kapacitor166)
-	[`kapacitor:1.6.6-alpine`](#kapacitor166-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:6e1a8dd8042cfa5045eb150fc767a748b1f2ae19b827ecadf1951834d6b99798
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:d0343c030845d9b7cd35733afd6b1b4b5364be21bfafe89db45baea3ac20f564
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.7 MB (103742294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6805e77d4476e03d7febd30c68bdb00354f6a5fa9ee7c127a620ff094e3a3c30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 02:38:41 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 02 Jun 2023 02:38:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 02 Jun 2023 02:38:42 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 02 Jun 2023 02:38:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 02 Jun 2023 02:38:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 02 Jun 2023 02:38:47 GMT
EXPOSE 9092
# Fri, 02 Jun 2023 02:38:47 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 02 Jun 2023 02:38:47 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 02 Jun 2023 02:38:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jun 2023 02:38:47 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbffcb96dc632d76384e539be718964baeb572c659cf55dc796674ac903fcb8`  
		Last Modified: Fri, 02 Jun 2023 00:49:43 GMT  
		Size: 7.1 MB (7119010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f9a5c516c91d7365471a9adb64e10c74736d87fb7486a2f7071b44fd7fd7af`  
		Last Modified: Fri, 02 Jun 2023 02:39:21 GMT  
		Size: 29.0 MB (28957371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f17cc44f6e0f77e41e46672e5963f420603369ae1a03035bf741735cab7aa58`  
		Last Modified: Fri, 02 Jun 2023 02:39:18 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f409ef1583f0afb3889816873f66677baaa9bd9bd0564f36eefd76dc5f00843a`  
		Last Modified: Fri, 02 Jun 2023 02:39:23 GMT  
		Size: 37.2 MB (37233375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d961d7338fe472e2bf7a8dd84560f7fbb5dde4825ccf0118c1887d0f7873fefa`  
		Last Modified: Fri, 02 Jun 2023 02:39:18 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14c7901efdda252daad7f68695fc1d6f63f8603523f3fc85bd2140ad2caa103`  
		Last Modified: Fri, 02 Jun 2023 02:39:18 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:d13151a6503987a58dc1f7d5a01894efce72441a26beedc391cda3060b283477
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95849130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04fd6bc53791adfe9e2c5ff4da8dfcda78ced90459e50831d05bee380d33014e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:44:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 16 Jun 2023 01:44:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 16 Jun 2023 01:44:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 16 Jun 2023 01:44:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 16 Jun 2023 01:44:34 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 16 Jun 2023 01:44:34 GMT
EXPOSE 9092
# Fri, 16 Jun 2023 01:44:34 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 16 Jun 2023 01:44:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 16 Jun 2023 01:44:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 01:44:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:de11f41b5c8ee0d3b259584977df4adb3e9b005f95756baecf491f70b498f301`  
		Last Modified: Wed, 07 Jun 2023 02:07:45 GMT  
		Size: 27.0 MB (27026252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee26b726447e1212d998ed272bac5f848182c3b89be3e6af01eb0b854dcf5e5`  
		Last Modified: Fri, 16 Jun 2023 00:58:01 GMT  
		Size: 7.0 MB (7018740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9640a3f9f7900b6834742e387e60300dec7fef8d90772d5a6b24e39902e756c0`  
		Last Modified: Fri, 16 Jun 2023 01:44:43 GMT  
		Size: 27.0 MB (27001791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314e0ee4634c8b3c0ce266bca5933f53f45b4fd104e742e12d7d46044736c3b`  
		Last Modified: Fri, 16 Jun 2023 01:44:41 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76789ad8def01aaa402296cb241f8b46863be2ad0936c4c2301aa92415f4cdef`  
		Last Modified: Fri, 16 Jun 2023 01:44:45 GMT  
		Size: 34.8 MB (34800090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e74f709ea55a89d8d418ce46ae76fcd94ab005ea8864ec4084cdd613e8d99b1`  
		Last Modified: Fri, 16 Jun 2023 01:44:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ad107ec6ca82d482dc9aa06b7321226a5d68dfcd4376760ed3ae805adc6f9`  
		Last Modified: Fri, 16 Jun 2023 01:44:41 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:932638e8bd86b20ff4dd16a5714b915a6c4fb94e8780027aea47de69b176557d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97692479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49523c33f3f3b935aaecf9a83040a440775ec28bad5a10cd04621cc63e31309d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 04:16:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 16 Jun 2023 04:16:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 16 Jun 2023 04:16:05 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 16 Jun 2023 04:16:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 16 Jun 2023 04:16:10 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 16 Jun 2023 04:16:10 GMT
EXPOSE 9092
# Fri, 16 Jun 2023 04:16:10 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 16 Jun 2023 04:16:10 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 16 Jun 2023 04:16:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 04:16:10 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b9a6243b9acb8c363f380b1a38f24b474ba69e18bc9631b7e9ff2ac3eb086c`  
		Last Modified: Fri, 16 Jun 2023 02:33:46 GMT  
		Size: 7.1 MB (7066023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba606495bf99b9ad74ebff867d48e1f54c84caf7ff306df30e4579fd55a85ca6`  
		Last Modified: Fri, 16 Jun 2023 04:16:31 GMT  
		Size: 27.7 MB (27658991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64b05e162c49365d039083c3b45d345976f0193a879ab12f8fa52abde44f14a`  
		Last Modified: Fri, 16 Jun 2023 04:16:29 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85c8c15d2e3c32d5163ba0f3b2e6a3711d3a9c285a551d47523b6c6dc6565ba`  
		Last Modified: Fri, 16 Jun 2023 04:16:32 GMT  
		Size: 34.6 MB (34575998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358e4e6a3843f9b618bd8ebf49e50b8b86caceffadb03902e3f107c72c93272a`  
		Last Modified: Fri, 16 Jun 2023 04:16:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60673dcf6a7f6fe3c2036897110de2faae24a60b2df9b3155e7cace4099e86f`  
		Last Modified: Fri, 16 Jun 2023 04:16:29 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:2d4571bbd7f39b054949f82034b3d529b2bc0ccf3889e2e72a592d8560d57f7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:32b8cb0e1e1e3fda8e954b79cbe4e15272e04ba7427f841b22dff8cf0818ffcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22655711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552ce7bbe44c57a5913883fc98455db619d77b2a7bd7fdd412bbaa408e6b1f70`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:13:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 22:13:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 22:13:18 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 28 Apr 2023 23:22:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 28 Apr 2023 23:22:49 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 28 Apr 2023 23:22:49 GMT
EXPOSE 9092
# Fri, 28 Apr 2023 23:22:49 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 28 Apr 2023 23:22:49 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 28 Apr 2023 23:22:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 23:22:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def2ae1fee272a0a418749677679ac1c48b9f3e46f04d5e3d55629dbd23b873`  
		Last Modified: Fri, 28 Apr 2023 23:23:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3f0ea5f775510249983621f9e6d068315844c260e3ba78b54aa1e37c75da71`  
		Last Modified: Fri, 28 Apr 2023 23:23:37 GMT  
		Size: 284.6 KB (284590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e220a492f7218c87ce3c9e0650aadb41b9e6d0be6381444ca3cf4179c7096910`  
		Last Modified: Fri, 28 Apr 2023 23:23:40 GMT  
		Size: 19.5 MB (19540839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fbec329944aaf6c9f89ae7cece3270108a31045736265d990cb08932d5df88`  
		Last Modified: Fri, 28 Apr 2023 23:23:37 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9883d7baa7fdbc3080e127193f17ee34fa171270d67405174661e523128960fe`  
		Last Modified: Fri, 28 Apr 2023 23:23:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:6e1a8dd8042cfa5045eb150fc767a748b1f2ae19b827ecadf1951834d6b99798
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:d0343c030845d9b7cd35733afd6b1b4b5364be21bfafe89db45baea3ac20f564
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.7 MB (103742294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6805e77d4476e03d7febd30c68bdb00354f6a5fa9ee7c127a620ff094e3a3c30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 02:38:41 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 02 Jun 2023 02:38:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 02 Jun 2023 02:38:42 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 02 Jun 2023 02:38:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 02 Jun 2023 02:38:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 02 Jun 2023 02:38:47 GMT
EXPOSE 9092
# Fri, 02 Jun 2023 02:38:47 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 02 Jun 2023 02:38:47 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 02 Jun 2023 02:38:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jun 2023 02:38:47 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbffcb96dc632d76384e539be718964baeb572c659cf55dc796674ac903fcb8`  
		Last Modified: Fri, 02 Jun 2023 00:49:43 GMT  
		Size: 7.1 MB (7119010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f9a5c516c91d7365471a9adb64e10c74736d87fb7486a2f7071b44fd7fd7af`  
		Last Modified: Fri, 02 Jun 2023 02:39:21 GMT  
		Size: 29.0 MB (28957371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f17cc44f6e0f77e41e46672e5963f420603369ae1a03035bf741735cab7aa58`  
		Last Modified: Fri, 02 Jun 2023 02:39:18 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f409ef1583f0afb3889816873f66677baaa9bd9bd0564f36eefd76dc5f00843a`  
		Last Modified: Fri, 02 Jun 2023 02:39:23 GMT  
		Size: 37.2 MB (37233375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d961d7338fe472e2bf7a8dd84560f7fbb5dde4825ccf0118c1887d0f7873fefa`  
		Last Modified: Fri, 02 Jun 2023 02:39:18 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14c7901efdda252daad7f68695fc1d6f63f8603523f3fc85bd2140ad2caa103`  
		Last Modified: Fri, 02 Jun 2023 02:39:18 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:d13151a6503987a58dc1f7d5a01894efce72441a26beedc391cda3060b283477
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95849130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04fd6bc53791adfe9e2c5ff4da8dfcda78ced90459e50831d05bee380d33014e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:44:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 16 Jun 2023 01:44:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 16 Jun 2023 01:44:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 16 Jun 2023 01:44:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 16 Jun 2023 01:44:34 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 16 Jun 2023 01:44:34 GMT
EXPOSE 9092
# Fri, 16 Jun 2023 01:44:34 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 16 Jun 2023 01:44:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 16 Jun 2023 01:44:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 01:44:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:de11f41b5c8ee0d3b259584977df4adb3e9b005f95756baecf491f70b498f301`  
		Last Modified: Wed, 07 Jun 2023 02:07:45 GMT  
		Size: 27.0 MB (27026252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee26b726447e1212d998ed272bac5f848182c3b89be3e6af01eb0b854dcf5e5`  
		Last Modified: Fri, 16 Jun 2023 00:58:01 GMT  
		Size: 7.0 MB (7018740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9640a3f9f7900b6834742e387e60300dec7fef8d90772d5a6b24e39902e756c0`  
		Last Modified: Fri, 16 Jun 2023 01:44:43 GMT  
		Size: 27.0 MB (27001791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314e0ee4634c8b3c0ce266bca5933f53f45b4fd104e742e12d7d46044736c3b`  
		Last Modified: Fri, 16 Jun 2023 01:44:41 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76789ad8def01aaa402296cb241f8b46863be2ad0936c4c2301aa92415f4cdef`  
		Last Modified: Fri, 16 Jun 2023 01:44:45 GMT  
		Size: 34.8 MB (34800090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e74f709ea55a89d8d418ce46ae76fcd94ab005ea8864ec4084cdd613e8d99b1`  
		Last Modified: Fri, 16 Jun 2023 01:44:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ad107ec6ca82d482dc9aa06b7321226a5d68dfcd4376760ed3ae805adc6f9`  
		Last Modified: Fri, 16 Jun 2023 01:44:41 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:932638e8bd86b20ff4dd16a5714b915a6c4fb94e8780027aea47de69b176557d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97692479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49523c33f3f3b935aaecf9a83040a440775ec28bad5a10cd04621cc63e31309d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 04:16:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 16 Jun 2023 04:16:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 16 Jun 2023 04:16:05 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 16 Jun 2023 04:16:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 16 Jun 2023 04:16:10 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 16 Jun 2023 04:16:10 GMT
EXPOSE 9092
# Fri, 16 Jun 2023 04:16:10 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 16 Jun 2023 04:16:10 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 16 Jun 2023 04:16:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 04:16:10 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b9a6243b9acb8c363f380b1a38f24b474ba69e18bc9631b7e9ff2ac3eb086c`  
		Last Modified: Fri, 16 Jun 2023 02:33:46 GMT  
		Size: 7.1 MB (7066023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba606495bf99b9ad74ebff867d48e1f54c84caf7ff306df30e4579fd55a85ca6`  
		Last Modified: Fri, 16 Jun 2023 04:16:31 GMT  
		Size: 27.7 MB (27658991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64b05e162c49365d039083c3b45d345976f0193a879ab12f8fa52abde44f14a`  
		Last Modified: Fri, 16 Jun 2023 04:16:29 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85c8c15d2e3c32d5163ba0f3b2e6a3711d3a9c285a551d47523b6c6dc6565ba`  
		Last Modified: Fri, 16 Jun 2023 04:16:32 GMT  
		Size: 34.6 MB (34575998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358e4e6a3843f9b618bd8ebf49e50b8b86caceffadb03902e3f107c72c93272a`  
		Last Modified: Fri, 16 Jun 2023 04:16:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60673dcf6a7f6fe3c2036897110de2faae24a60b2df9b3155e7cace4099e86f`  
		Last Modified: Fri, 16 Jun 2023 04:16:29 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:2d4571bbd7f39b054949f82034b3d529b2bc0ccf3889e2e72a592d8560d57f7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:32b8cb0e1e1e3fda8e954b79cbe4e15272e04ba7427f841b22dff8cf0818ffcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22655711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552ce7bbe44c57a5913883fc98455db619d77b2a7bd7fdd412bbaa408e6b1f70`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:13:17 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 22:13:18 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 29 Mar 2023 22:13:18 GMT
ENV KAPACITOR_VERSION=1.5.9
# Fri, 28 Apr 2023 23:22:48 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 28 Apr 2023 23:22:49 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 28 Apr 2023 23:22:49 GMT
EXPOSE 9092
# Fri, 28 Apr 2023 23:22:49 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 28 Apr 2023 23:22:49 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 28 Apr 2023 23:22:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 23:22:49 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def2ae1fee272a0a418749677679ac1c48b9f3e46f04d5e3d55629dbd23b873`  
		Last Modified: Fri, 28 Apr 2023 23:23:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3f0ea5f775510249983621f9e6d068315844c260e3ba78b54aa1e37c75da71`  
		Last Modified: Fri, 28 Apr 2023 23:23:37 GMT  
		Size: 284.6 KB (284590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e220a492f7218c87ce3c9e0650aadb41b9e6d0be6381444ca3cf4179c7096910`  
		Last Modified: Fri, 28 Apr 2023 23:23:40 GMT  
		Size: 19.5 MB (19540839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fbec329944aaf6c9f89ae7cece3270108a31045736265d990cb08932d5df88`  
		Last Modified: Fri, 28 Apr 2023 23:23:37 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9883d7baa7fdbc3080e127193f17ee34fa171270d67405174661e523128960fe`  
		Last Modified: Fri, 28 Apr 2023 23:23:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:55856418d171f20e0df942a207ec2fb872a66bf0547c02079d5828cf3a38ee1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:ef549009b89c03029ebda4b096a0677fc21903fa8df9a8335b3809c90e5b9699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132179319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa06f2cd7551619396b7af826f2e1c367f03ff9aebb3275248c9085a96607ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 02:38:41 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 02 Jun 2023 02:38:52 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 02 Jun 2023 02:39:05 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 02 Jun 2023 02:39:05 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 02 Jun 2023 02:39:05 GMT
EXPOSE 9092
# Fri, 02 Jun 2023 02:39:05 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 02 Jun 2023 02:39:05 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 02 Jun 2023 02:39:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jun 2023 02:39:05 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbffcb96dc632d76384e539be718964baeb572c659cf55dc796674ac903fcb8`  
		Last Modified: Fri, 02 Jun 2023 00:49:43 GMT  
		Size: 7.1 MB (7119010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f9a5c516c91d7365471a9adb64e10c74736d87fb7486a2f7071b44fd7fd7af`  
		Last Modified: Fri, 02 Jun 2023 02:39:21 GMT  
		Size: 29.0 MB (28957371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b65c9fb6ac95a427fc262b5761ecedefcd0f22eb2825a19d8db4f306d41f84`  
		Last Modified: Fri, 02 Jun 2023 02:39:39 GMT  
		Size: 65.7 MB (65672205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69856d7ad155fe70cbf44fabd7588ae02c671b7b45ad585b0e413245ffe142b1`  
		Last Modified: Fri, 02 Jun 2023 02:39:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c5902e91c97acc79a95c02da71b2f53bb00fec5453b055f258808123e8dbbf`  
		Last Modified: Fri, 02 Jun 2023 02:39:31 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:d5f48ebfdaf1f5b309b0530a263d9954796a5ab427201a4d29ea722f81559f68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124784419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9044dbc53d0d3ddeec7e05f2384b438e7b07f66f32fd9cf5d3fca7bd21a82940`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 04:16:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 16 Jun 2023 04:16:12 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 16 Jun 2023 04:16:18 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 16 Jun 2023 04:16:18 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 16 Jun 2023 04:16:18 GMT
EXPOSE 9092
# Fri, 16 Jun 2023 04:16:19 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 16 Jun 2023 04:16:19 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 16 Jun 2023 04:16:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 04:16:19 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b9a6243b9acb8c363f380b1a38f24b474ba69e18bc9631b7e9ff2ac3eb086c`  
		Last Modified: Fri, 16 Jun 2023 02:33:46 GMT  
		Size: 7.1 MB (7066023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba606495bf99b9ad74ebff867d48e1f54c84caf7ff306df30e4579fd55a85ca6`  
		Last Modified: Fri, 16 Jun 2023 04:16:31 GMT  
		Size: 27.7 MB (27658991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a00cf39cbfb3c07898e664ea782061618ec493892046f32c76d59ab42d94c10`  
		Last Modified: Fri, 16 Jun 2023 04:16:46 GMT  
		Size: 61.7 MB (61669748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f11e5002b3deab9330d776dfdbc49b1cebf954e6441cb2fc56634b8f3817ea5`  
		Last Modified: Fri, 16 Jun 2023 04:16:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346adb05d865f78200cd639d8b3aa4338d23a1b2dd64863b96f3c0a613f44341`  
		Last Modified: Fri, 16 Jun 2023 04:16:41 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:5b3a23f43f032563c2e74a4f17b26859edee50d357398c8e27c383a4affb1f39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:5ecb6d70b04f682bf083d8221c8795d515e8f2e62c6e0e17fef78979526ae968
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784aac51c22cb50998a5cfeae53ed762fb5e682c162cbf975702f0503c544e3d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:45:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 05:45:39 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 05:45:39 GMT
ENV KAPACITOR_VERSION=1.6.6
# Thu, 15 Jun 2023 05:45:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 05:45:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 15 Jun 2023 05:45:47 GMT
EXPOSE 9092
# Thu, 15 Jun 2023 05:45:47 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 15 Jun 2023 05:45:47 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 15 Jun 2023 05:45:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 05:45:47 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a8fc827b52bde08700ba04f00ff102db063e64c9d6f58f80884614a4b18b6`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186b7f8de181d743078167f2d739bd3193478b6397835fbb848f6ab306c97436`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 284.9 KB (284893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292743d14620badd8bc64815855e5e1a3e6eee5de1a6575b872a44baeda0c653`  
		Last Modified: Thu, 15 Jun 2023 05:46:09 GMT  
		Size: 65.6 MB (65580144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f31ef8d9aedecbc7b151c5648728c4832769030d32ab5d4e65bec55660b71a`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6cc3af6c1f536187a6654c62310d508785834956452dc211a66ca74ff7d452`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.6`

```console
$ docker pull kapacitor@sha256:55856418d171f20e0df942a207ec2fb872a66bf0547c02079d5828cf3a38ee1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:ef549009b89c03029ebda4b096a0677fc21903fa8df9a8335b3809c90e5b9699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132179319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa06f2cd7551619396b7af826f2e1c367f03ff9aebb3275248c9085a96607ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 02:38:41 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 02 Jun 2023 02:38:52 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 02 Jun 2023 02:39:05 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 02 Jun 2023 02:39:05 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 02 Jun 2023 02:39:05 GMT
EXPOSE 9092
# Fri, 02 Jun 2023 02:39:05 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 02 Jun 2023 02:39:05 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 02 Jun 2023 02:39:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jun 2023 02:39:05 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbffcb96dc632d76384e539be718964baeb572c659cf55dc796674ac903fcb8`  
		Last Modified: Fri, 02 Jun 2023 00:49:43 GMT  
		Size: 7.1 MB (7119010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f9a5c516c91d7365471a9adb64e10c74736d87fb7486a2f7071b44fd7fd7af`  
		Last Modified: Fri, 02 Jun 2023 02:39:21 GMT  
		Size: 29.0 MB (28957371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b65c9fb6ac95a427fc262b5761ecedefcd0f22eb2825a19d8db4f306d41f84`  
		Last Modified: Fri, 02 Jun 2023 02:39:39 GMT  
		Size: 65.7 MB (65672205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69856d7ad155fe70cbf44fabd7588ae02c671b7b45ad585b0e413245ffe142b1`  
		Last Modified: Fri, 02 Jun 2023 02:39:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c5902e91c97acc79a95c02da71b2f53bb00fec5453b055f258808123e8dbbf`  
		Last Modified: Fri, 02 Jun 2023 02:39:31 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:d5f48ebfdaf1f5b309b0530a263d9954796a5ab427201a4d29ea722f81559f68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124784419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9044dbc53d0d3ddeec7e05f2384b438e7b07f66f32fd9cf5d3fca7bd21a82940`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 04:16:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 16 Jun 2023 04:16:12 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 16 Jun 2023 04:16:18 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 16 Jun 2023 04:16:18 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 16 Jun 2023 04:16:18 GMT
EXPOSE 9092
# Fri, 16 Jun 2023 04:16:19 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 16 Jun 2023 04:16:19 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 16 Jun 2023 04:16:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 04:16:19 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b9a6243b9acb8c363f380b1a38f24b474ba69e18bc9631b7e9ff2ac3eb086c`  
		Last Modified: Fri, 16 Jun 2023 02:33:46 GMT  
		Size: 7.1 MB (7066023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba606495bf99b9ad74ebff867d48e1f54c84caf7ff306df30e4579fd55a85ca6`  
		Last Modified: Fri, 16 Jun 2023 04:16:31 GMT  
		Size: 27.7 MB (27658991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a00cf39cbfb3c07898e664ea782061618ec493892046f32c76d59ab42d94c10`  
		Last Modified: Fri, 16 Jun 2023 04:16:46 GMT  
		Size: 61.7 MB (61669748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f11e5002b3deab9330d776dfdbc49b1cebf954e6441cb2fc56634b8f3817ea5`  
		Last Modified: Fri, 16 Jun 2023 04:16:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346adb05d865f78200cd639d8b3aa4338d23a1b2dd64863b96f3c0a613f44341`  
		Last Modified: Fri, 16 Jun 2023 04:16:41 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.6-alpine`

```console
$ docker pull kapacitor@sha256:5b3a23f43f032563c2e74a4f17b26859edee50d357398c8e27c383a4affb1f39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:5ecb6d70b04f682bf083d8221c8795d515e8f2e62c6e0e17fef78979526ae968
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784aac51c22cb50998a5cfeae53ed762fb5e682c162cbf975702f0503c544e3d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:45:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 05:45:39 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 05:45:39 GMT
ENV KAPACITOR_VERSION=1.6.6
# Thu, 15 Jun 2023 05:45:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 05:45:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 15 Jun 2023 05:45:47 GMT
EXPOSE 9092
# Thu, 15 Jun 2023 05:45:47 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 15 Jun 2023 05:45:47 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 15 Jun 2023 05:45:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 05:45:47 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a8fc827b52bde08700ba04f00ff102db063e64c9d6f58f80884614a4b18b6`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186b7f8de181d743078167f2d739bd3193478b6397835fbb848f6ab306c97436`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 284.9 KB (284893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292743d14620badd8bc64815855e5e1a3e6eee5de1a6575b872a44baeda0c653`  
		Last Modified: Thu, 15 Jun 2023 05:46:09 GMT  
		Size: 65.6 MB (65580144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f31ef8d9aedecbc7b151c5648728c4832769030d32ab5d4e65bec55660b71a`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6cc3af6c1f536187a6654c62310d508785834956452dc211a66ca74ff7d452`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:5b3a23f43f032563c2e74a4f17b26859edee50d357398c8e27c383a4affb1f39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:5ecb6d70b04f682bf083d8221c8795d515e8f2e62c6e0e17fef78979526ae968
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784aac51c22cb50998a5cfeae53ed762fb5e682c162cbf975702f0503c544e3d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:45:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 05:45:39 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 15 Jun 2023 05:45:39 GMT
ENV KAPACITOR_VERSION=1.6.6
# Thu, 15 Jun 2023 05:45:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 15 Jun 2023 05:45:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Thu, 15 Jun 2023 05:45:47 GMT
EXPOSE 9092
# Thu, 15 Jun 2023 05:45:47 GMT
VOLUME [/var/lib/kapacitor]
# Thu, 15 Jun 2023 05:45:47 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Thu, 15 Jun 2023 05:45:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 05:45:47 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a8fc827b52bde08700ba04f00ff102db063e64c9d6f58f80884614a4b18b6`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186b7f8de181d743078167f2d739bd3193478b6397835fbb848f6ab306c97436`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 284.9 KB (284893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292743d14620badd8bc64815855e5e1a3e6eee5de1a6575b872a44baeda0c653`  
		Last Modified: Thu, 15 Jun 2023 05:46:09 GMT  
		Size: 65.6 MB (65580144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f31ef8d9aedecbc7b151c5648728c4832769030d32ab5d4e65bec55660b71a`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6cc3af6c1f536187a6654c62310d508785834956452dc211a66ca74ff7d452`  
		Last Modified: Thu, 15 Jun 2023 05:46:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:55856418d171f20e0df942a207ec2fb872a66bf0547c02079d5828cf3a38ee1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:ef549009b89c03029ebda4b096a0677fc21903fa8df9a8335b3809c90e5b9699
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132179319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fa06f2cd7551619396b7af826f2e1c367f03ff9aebb3275248c9085a96607ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 00:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 02:38:41 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 02 Jun 2023 02:38:52 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 02 Jun 2023 02:39:05 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 02 Jun 2023 02:39:05 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 02 Jun 2023 02:39:05 GMT
EXPOSE 9092
# Fri, 02 Jun 2023 02:39:05 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 02 Jun 2023 02:39:05 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 02 Jun 2023 02:39:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jun 2023 02:39:05 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbffcb96dc632d76384e539be718964baeb572c659cf55dc796674ac903fcb8`  
		Last Modified: Fri, 02 Jun 2023 00:49:43 GMT  
		Size: 7.1 MB (7119010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f9a5c516c91d7365471a9adb64e10c74736d87fb7486a2f7071b44fd7fd7af`  
		Last Modified: Fri, 02 Jun 2023 02:39:21 GMT  
		Size: 29.0 MB (28957371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b65c9fb6ac95a427fc262b5761ecedefcd0f22eb2825a19d8db4f306d41f84`  
		Last Modified: Fri, 02 Jun 2023 02:39:39 GMT  
		Size: 65.7 MB (65672205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69856d7ad155fe70cbf44fabd7588ae02c671b7b45ad585b0e413245ffe142b1`  
		Last Modified: Fri, 02 Jun 2023 02:39:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c5902e91c97acc79a95c02da71b2f53bb00fec5453b055f258808123e8dbbf`  
		Last Modified: Fri, 02 Jun 2023 02:39:31 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:d5f48ebfdaf1f5b309b0530a263d9954796a5ab427201a4d29ea722f81559f68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124784419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9044dbc53d0d3ddeec7e05f2384b438e7b07f66f32fd9cf5d3fca7bd21a82940`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 04:16:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Fri, 16 Jun 2023 04:16:12 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 16 Jun 2023 04:16:18 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Fri, 16 Jun 2023 04:16:18 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 16 Jun 2023 04:16:18 GMT
EXPOSE 9092
# Fri, 16 Jun 2023 04:16:19 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 16 Jun 2023 04:16:19 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Fri, 16 Jun 2023 04:16:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 04:16:19 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b9a6243b9acb8c363f380b1a38f24b474ba69e18bc9631b7e9ff2ac3eb086c`  
		Last Modified: Fri, 16 Jun 2023 02:33:46 GMT  
		Size: 7.1 MB (7066023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba606495bf99b9ad74ebff867d48e1f54c84caf7ff306df30e4579fd55a85ca6`  
		Last Modified: Fri, 16 Jun 2023 04:16:31 GMT  
		Size: 27.7 MB (27658991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a00cf39cbfb3c07898e664ea782061618ec493892046f32c76d59ab42d94c10`  
		Last Modified: Fri, 16 Jun 2023 04:16:46 GMT  
		Size: 61.7 MB (61669748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f11e5002b3deab9330d776dfdbc49b1cebf954e6441cb2fc56634b8f3817ea5`  
		Last Modified: Fri, 16 Jun 2023 04:16:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346adb05d865f78200cd639d8b3aa4338d23a1b2dd64863b96f3c0a613f44341`  
		Last Modified: Fri, 16 Jun 2023 04:16:41 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
