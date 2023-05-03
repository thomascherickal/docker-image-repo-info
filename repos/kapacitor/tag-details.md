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
$ docker pull kapacitor@sha256:f3ecdb09c20d4b4c36946a416be94dd4b7f7ab782a4fac44512170c28415b5c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:a358d3a92e40341d8bc3023459b2a1992f6f5b34f6f8ae7d2289426a27d083e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106141288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ae42c2ad0cbaa53ecfa9eb900cd773e4628a3ef6a47af12f95d309248914d9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:26:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 16:09:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 16:09:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 16:09:23 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 03 May 2023 16:09:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 16:09:27 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 16:09:27 GMT
EXPOSE 9092
# Wed, 03 May 2023 16:09:27 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 16:09:27 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 16:09:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 16:09:27 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade6d81308cf88645476bddfaa8c5c2be767c77660b156a2bc5e740cd906431b`  
		Last Modified: Tue, 02 May 2023 23:43:33 GMT  
		Size: 7.1 MB (7123825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb507a78420a94908f02595d22f75332c5c8693df6cd0154f4e78a78ec2c12f2`  
		Last Modified: Wed, 03 May 2023 16:09:58 GMT  
		Size: 31.4 MB (31351810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb81e302e1955811630efd33259ba9a8358b5e7c2558242943d7291ec0f8cd9f`  
		Last Modified: Wed, 03 May 2023 16:09:55 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab73c608a4d388fa3539471b9d70a72d0614cc0a8f220f4b32499d31f46bf85`  
		Last Modified: Wed, 03 May 2023 16:10:00 GMT  
		Size: 37.2 MB (37233440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d9adada2985946ccf06d8a7231e31bebf58a0ddc2bb27aa53f70d6b543e616`  
		Last Modified: Wed, 03 May 2023 16:09:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81479b1c5175bfde4b5406c0a8b09e54bbffd7d85035badae694012d0d86b678`  
		Last Modified: Wed, 03 May 2023 16:09:55 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:efe2b043634dd52c16f731209dffe21fcbe5013facdbfeef154e79e4133dd2cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.1 MB (96075285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d7076b015359b8b58ad28668e220cd7a9f2b3000849d1ad5864a18002fa085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:18:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:49:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 17:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 17:50:01 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 03 May 2023 17:50:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 17:50:06 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 17:50:06 GMT
EXPOSE 9092
# Wed, 03 May 2023 17:50:06 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 17:50:06 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 17:50:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 17:50:06 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504c6da4089db5ac53834d607cde1276a5357b31bde8bc60fd8fcfd996843ebe`  
		Last Modified: Tue, 02 May 2023 23:41:43 GMT  
		Size: 7.0 MB (7022848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8dfae1d36232a8a8ae0dd83a6caa7c0b18e24bb4ca25b53d5eaa9c1d25c4ee`  
		Last Modified: Wed, 03 May 2023 17:50:18 GMT  
		Size: 27.2 MB (27224213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efb2e55056d6d8be2dc332d35f582547bf9ae687703a321f246ebe507f35ce9`  
		Last Modified: Wed, 03 May 2023 17:50:15 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84ce729dd79f5cd0fa33bd3b3f4c895aeed36c58bc262dd8aa13e83009ecfd8`  
		Last Modified: Wed, 03 May 2023 17:50:20 GMT  
		Size: 34.8 MB (34800576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5917f26f795c8664ee49fa675eff6db84ad942f43786eef05b87222031f5a7`  
		Last Modified: Wed, 03 May 2023 17:50:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51af083a02f637aa1160f3e3bf503f4791a82599f23f23aba10791ec12351aab`  
		Last Modified: Wed, 03 May 2023 17:50:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:b8711acf525dbe951dd8d9981b5c7e2a8e7da3e0c3ca37a53aad9085137d1268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98903179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab55619000c54caef705f9032620fb320118a17fe9af74853ed8626810f28d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:56:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:10:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 14:10:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 14:10:11 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 03 May 2023 14:10:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 14:10:16 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 14:10:16 GMT
EXPOSE 9092
# Wed, 03 May 2023 14:10:16 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 14:10:16 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 14:10:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 14:10:16 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1026f845342a6b9d1ce7fd9eafb77e2f1f29edebd77279101a8dbcf8c6d9dc1d`  
		Last Modified: Wed, 03 May 2023 00:15:25 GMT  
		Size: 7.1 MB (7065779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d123d3a8b02a77eaa4722bc4519550be04423f94bd1a64d9766c78b317e499`  
		Last Modified: Wed, 03 May 2023 14:10:36 GMT  
		Size: 28.9 MB (28872127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf7e50a4f7858da5cc9420295d9d17a826b890b18ef1d5f19475bfde23f71d1`  
		Last Modified: Wed, 03 May 2023 14:10:34 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1592c7bb03acfe466209314c572b7ec61204fff685781f32fad726f029ac73`  
		Last Modified: Wed, 03 May 2023 14:10:37 GMT  
		Size: 34.6 MB (34575464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e021f6a753a30cd3b9c2ddc3c7e18f161e2ff548f9a1856b5398247b99a26`  
		Last Modified: Wed, 03 May 2023 14:10:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06362168737b9f2d1065fff0c60b30d6a908b0e1f94e30f032087c4af7e3dec9`  
		Last Modified: Wed, 03 May 2023 14:10:33 GMT  
		Size: 232.0 B  
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
$ docker pull kapacitor@sha256:f3ecdb09c20d4b4c36946a416be94dd4b7f7ab782a4fac44512170c28415b5c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:a358d3a92e40341d8bc3023459b2a1992f6f5b34f6f8ae7d2289426a27d083e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106141288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10ae42c2ad0cbaa53ecfa9eb900cd773e4628a3ef6a47af12f95d309248914d9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:26:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 16:09:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 16:09:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 16:09:23 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 03 May 2023 16:09:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 16:09:27 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 16:09:27 GMT
EXPOSE 9092
# Wed, 03 May 2023 16:09:27 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 16:09:27 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 16:09:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 16:09:27 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade6d81308cf88645476bddfaa8c5c2be767c77660b156a2bc5e740cd906431b`  
		Last Modified: Tue, 02 May 2023 23:43:33 GMT  
		Size: 7.1 MB (7123825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb507a78420a94908f02595d22f75332c5c8693df6cd0154f4e78a78ec2c12f2`  
		Last Modified: Wed, 03 May 2023 16:09:58 GMT  
		Size: 31.4 MB (31351810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb81e302e1955811630efd33259ba9a8358b5e7c2558242943d7291ec0f8cd9f`  
		Last Modified: Wed, 03 May 2023 16:09:55 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab73c608a4d388fa3539471b9d70a72d0614cc0a8f220f4b32499d31f46bf85`  
		Last Modified: Wed, 03 May 2023 16:10:00 GMT  
		Size: 37.2 MB (37233440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d9adada2985946ccf06d8a7231e31bebf58a0ddc2bb27aa53f70d6b543e616`  
		Last Modified: Wed, 03 May 2023 16:09:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81479b1c5175bfde4b5406c0a8b09e54bbffd7d85035badae694012d0d86b678`  
		Last Modified: Wed, 03 May 2023 16:09:55 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:efe2b043634dd52c16f731209dffe21fcbe5013facdbfeef154e79e4133dd2cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.1 MB (96075285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d7076b015359b8b58ad28668e220cd7a9f2b3000849d1ad5864a18002fa085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:18:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:49:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 17:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 17:50:01 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 03 May 2023 17:50:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 17:50:06 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 17:50:06 GMT
EXPOSE 9092
# Wed, 03 May 2023 17:50:06 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 17:50:06 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 17:50:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 17:50:06 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504c6da4089db5ac53834d607cde1276a5357b31bde8bc60fd8fcfd996843ebe`  
		Last Modified: Tue, 02 May 2023 23:41:43 GMT  
		Size: 7.0 MB (7022848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8dfae1d36232a8a8ae0dd83a6caa7c0b18e24bb4ca25b53d5eaa9c1d25c4ee`  
		Last Modified: Wed, 03 May 2023 17:50:18 GMT  
		Size: 27.2 MB (27224213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efb2e55056d6d8be2dc332d35f582547bf9ae687703a321f246ebe507f35ce9`  
		Last Modified: Wed, 03 May 2023 17:50:15 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84ce729dd79f5cd0fa33bd3b3f4c895aeed36c58bc262dd8aa13e83009ecfd8`  
		Last Modified: Wed, 03 May 2023 17:50:20 GMT  
		Size: 34.8 MB (34800576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5917f26f795c8664ee49fa675eff6db84ad942f43786eef05b87222031f5a7`  
		Last Modified: Wed, 03 May 2023 17:50:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51af083a02f637aa1160f3e3bf503f4791a82599f23f23aba10791ec12351aab`  
		Last Modified: Wed, 03 May 2023 17:50:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:b8711acf525dbe951dd8d9981b5c7e2a8e7da3e0c3ca37a53aad9085137d1268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98903179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab55619000c54caef705f9032620fb320118a17fe9af74853ed8626810f28d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:56:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:10:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 14:10:11 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 14:10:11 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 03 May 2023 14:10:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 14:10:16 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 14:10:16 GMT
EXPOSE 9092
# Wed, 03 May 2023 14:10:16 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 14:10:16 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 14:10:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 14:10:16 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1026f845342a6b9d1ce7fd9eafb77e2f1f29edebd77279101a8dbcf8c6d9dc1d`  
		Last Modified: Wed, 03 May 2023 00:15:25 GMT  
		Size: 7.1 MB (7065779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d123d3a8b02a77eaa4722bc4519550be04423f94bd1a64d9766c78b317e499`  
		Last Modified: Wed, 03 May 2023 14:10:36 GMT  
		Size: 28.9 MB (28872127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf7e50a4f7858da5cc9420295d9d17a826b890b18ef1d5f19475bfde23f71d1`  
		Last Modified: Wed, 03 May 2023 14:10:34 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1592c7bb03acfe466209314c572b7ec61204fff685781f32fad726f029ac73`  
		Last Modified: Wed, 03 May 2023 14:10:37 GMT  
		Size: 34.6 MB (34575464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e021f6a753a30cd3b9c2ddc3c7e18f161e2ff548f9a1856b5398247b99a26`  
		Last Modified: Wed, 03 May 2023 14:10:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06362168737b9f2d1065fff0c60b30d6a908b0e1f94e30f032087c4af7e3dec9`  
		Last Modified: Wed, 03 May 2023 14:10:33 GMT  
		Size: 232.0 B  
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
$ docker pull kapacitor@sha256:3bc937bcd57a9eb476aa10e059ad331407fb7b7f787ccfcb577a941a2b405bed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:a4b03b00a2a79ddd0030143fe32c39ec8722b5eb6262eaa3d6e0278b62e73696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134578250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b48dbd6cef9c910481ef128df68501a0650fcbfcccb27106f370336706132bc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:26:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 16:09:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 16:09:31 GMT
ENV KAPACITOR_VERSION=1.6.6
# Wed, 03 May 2023 16:09:42 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 16:09:42 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 16:09:42 GMT
EXPOSE 9092
# Wed, 03 May 2023 16:09:42 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 16:09:42 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 16:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 16:09:42 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade6d81308cf88645476bddfaa8c5c2be767c77660b156a2bc5e740cd906431b`  
		Last Modified: Tue, 02 May 2023 23:43:33 GMT  
		Size: 7.1 MB (7123825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb507a78420a94908f02595d22f75332c5c8693df6cd0154f4e78a78ec2c12f2`  
		Last Modified: Wed, 03 May 2023 16:09:58 GMT  
		Size: 31.4 MB (31351810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e0cd46b31d30fa84eb9b19625e6f729983f718960a32c93c5fe9cc8bd2e50c`  
		Last Modified: Wed, 03 May 2023 16:10:23 GMT  
		Size: 65.7 MB (65672194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120ea54647ec099a9b19129b4b91135f5ddb6073750d64a731feca9b2c2dfd8`  
		Last Modified: Wed, 03 May 2023 16:10:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7cee67f7a88d03d99a4e6bbbadfd77e7964a038d55adcdcbb3408582942834`  
		Last Modified: Wed, 03 May 2023 16:10:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:fd8637c1228eb50cf5f9a226f86d175e705572f38053eba3d4058eee650929bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125995091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d6c6598cff035de8737c99fe263363e373c50e88d82380cf960e953220d02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:56:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:10:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 14:10:18 GMT
ENV KAPACITOR_VERSION=1.6.6
# Wed, 03 May 2023 14:10:24 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 14:10:25 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 14:10:25 GMT
EXPOSE 9092
# Wed, 03 May 2023 14:10:25 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 14:10:25 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 14:10:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 14:10:25 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1026f845342a6b9d1ce7fd9eafb77e2f1f29edebd77279101a8dbcf8c6d9dc1d`  
		Last Modified: Wed, 03 May 2023 00:15:25 GMT  
		Size: 7.1 MB (7065779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d123d3a8b02a77eaa4722bc4519550be04423f94bd1a64d9766c78b317e499`  
		Last Modified: Wed, 03 May 2023 14:10:36 GMT  
		Size: 28.9 MB (28872127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda45cfde5f7e38f5448246f9f11a613c4f44d625ba7d09c12190c77e3d64a2d`  
		Last Modified: Wed, 03 May 2023 14:10:50 GMT  
		Size: 61.7 MB (61669174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2f1193370470f52effdf853b25fe024dcb454fd638faf54c8205ecd57c3450`  
		Last Modified: Wed, 03 May 2023 14:10:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7bf8ddec5971b38e6b568b3e0c344e51318ca96c8955f2a7dadb0f3f689983`  
		Last Modified: Wed, 03 May 2023 14:10:44 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:ae18d242a2c3e38dab667b058e6e1c1c32db3985089eb07bbff7a1124749fc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:73bb692306ea33eecba6040c0e63819c1ae048c49186a6f2c80c7d3eb6cc2c0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084421861cb41acf17a0a5c19fa524a1cd1b2233e96cbb6554bcae217c7543b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:13:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 22:13:56 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 28 Apr 2023 23:23:01 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 28 Apr 2023 23:23:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 28 Apr 2023 23:23:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 28 Apr 2023 23:23:12 GMT
EXPOSE 9092
# Fri, 28 Apr 2023 23:23:12 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 28 Apr 2023 23:23:12 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 28 Apr 2023 23:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 23:23:13 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562ec21068704bb8efd8a6db94153756f2ea649fc15b7a3d8c5ae495403deaff`  
		Last Modified: Fri, 28 Apr 2023 23:24:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d500101053a8592e41f90d59292cd74a1d55daea7ae9ae255f54f3c3b0bafa0`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 284.8 KB (284768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f632df2bffbd0c0aef5f148bd642609bbd3769c3a2f68af212c24569fe3059`  
		Last Modified: Fri, 28 Apr 2023 23:24:14 GMT  
		Size: 65.6 MB (65580141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe03849db0a97866932a7b703905538b0d9190b841dbc50e49d72d1840cf605`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f533d079920207448963e4c621b57d4b0faad5d7eabc65bf0171e777ec58e465`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.6`

```console
$ docker pull kapacitor@sha256:3bc937bcd57a9eb476aa10e059ad331407fb7b7f787ccfcb577a941a2b405bed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:a4b03b00a2a79ddd0030143fe32c39ec8722b5eb6262eaa3d6e0278b62e73696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134578250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b48dbd6cef9c910481ef128df68501a0650fcbfcccb27106f370336706132bc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:26:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 16:09:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 16:09:31 GMT
ENV KAPACITOR_VERSION=1.6.6
# Wed, 03 May 2023 16:09:42 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 16:09:42 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 16:09:42 GMT
EXPOSE 9092
# Wed, 03 May 2023 16:09:42 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 16:09:42 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 16:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 16:09:42 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade6d81308cf88645476bddfaa8c5c2be767c77660b156a2bc5e740cd906431b`  
		Last Modified: Tue, 02 May 2023 23:43:33 GMT  
		Size: 7.1 MB (7123825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb507a78420a94908f02595d22f75332c5c8693df6cd0154f4e78a78ec2c12f2`  
		Last Modified: Wed, 03 May 2023 16:09:58 GMT  
		Size: 31.4 MB (31351810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e0cd46b31d30fa84eb9b19625e6f729983f718960a32c93c5fe9cc8bd2e50c`  
		Last Modified: Wed, 03 May 2023 16:10:23 GMT  
		Size: 65.7 MB (65672194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120ea54647ec099a9b19129b4b91135f5ddb6073750d64a731feca9b2c2dfd8`  
		Last Modified: Wed, 03 May 2023 16:10:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7cee67f7a88d03d99a4e6bbbadfd77e7964a038d55adcdcbb3408582942834`  
		Last Modified: Wed, 03 May 2023 16:10:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:fd8637c1228eb50cf5f9a226f86d175e705572f38053eba3d4058eee650929bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125995091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d6c6598cff035de8737c99fe263363e373c50e88d82380cf960e953220d02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:56:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:10:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 14:10:18 GMT
ENV KAPACITOR_VERSION=1.6.6
# Wed, 03 May 2023 14:10:24 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 14:10:25 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 14:10:25 GMT
EXPOSE 9092
# Wed, 03 May 2023 14:10:25 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 14:10:25 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 14:10:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 14:10:25 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1026f845342a6b9d1ce7fd9eafb77e2f1f29edebd77279101a8dbcf8c6d9dc1d`  
		Last Modified: Wed, 03 May 2023 00:15:25 GMT  
		Size: 7.1 MB (7065779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d123d3a8b02a77eaa4722bc4519550be04423f94bd1a64d9766c78b317e499`  
		Last Modified: Wed, 03 May 2023 14:10:36 GMT  
		Size: 28.9 MB (28872127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda45cfde5f7e38f5448246f9f11a613c4f44d625ba7d09c12190c77e3d64a2d`  
		Last Modified: Wed, 03 May 2023 14:10:50 GMT  
		Size: 61.7 MB (61669174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2f1193370470f52effdf853b25fe024dcb454fd638faf54c8205ecd57c3450`  
		Last Modified: Wed, 03 May 2023 14:10:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7bf8ddec5971b38e6b568b3e0c344e51318ca96c8955f2a7dadb0f3f689983`  
		Last Modified: Wed, 03 May 2023 14:10:44 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.6-alpine`

```console
$ docker pull kapacitor@sha256:ae18d242a2c3e38dab667b058e6e1c1c32db3985089eb07bbff7a1124749fc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:73bb692306ea33eecba6040c0e63819c1ae048c49186a6f2c80c7d3eb6cc2c0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084421861cb41acf17a0a5c19fa524a1cd1b2233e96cbb6554bcae217c7543b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:13:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 22:13:56 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 28 Apr 2023 23:23:01 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 28 Apr 2023 23:23:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 28 Apr 2023 23:23:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 28 Apr 2023 23:23:12 GMT
EXPOSE 9092
# Fri, 28 Apr 2023 23:23:12 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 28 Apr 2023 23:23:12 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 28 Apr 2023 23:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 23:23:13 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562ec21068704bb8efd8a6db94153756f2ea649fc15b7a3d8c5ae495403deaff`  
		Last Modified: Fri, 28 Apr 2023 23:24:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d500101053a8592e41f90d59292cd74a1d55daea7ae9ae255f54f3c3b0bafa0`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 284.8 KB (284768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f632df2bffbd0c0aef5f148bd642609bbd3769c3a2f68af212c24569fe3059`  
		Last Modified: Fri, 28 Apr 2023 23:24:14 GMT  
		Size: 65.6 MB (65580141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe03849db0a97866932a7b703905538b0d9190b841dbc50e49d72d1840cf605`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f533d079920207448963e4c621b57d4b0faad5d7eabc65bf0171e777ec58e465`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:ae18d242a2c3e38dab667b058e6e1c1c32db3985089eb07bbff7a1124749fc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:73bb692306ea33eecba6040c0e63819c1ae048c49186a6f2c80c7d3eb6cc2c0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68673446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084421861cb41acf17a0a5c19fa524a1cd1b2233e96cbb6554bcae217c7543b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:13:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 29 Mar 2023 22:13:56 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Fri, 28 Apr 2023 23:23:01 GMT
ENV KAPACITOR_VERSION=1.6.6
# Fri, 28 Apr 2023 23:23:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     cp -ar /usr/src/kapacitor-*/* / &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 28 Apr 2023 23:23:12 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Fri, 28 Apr 2023 23:23:12 GMT
EXPOSE 9092
# Fri, 28 Apr 2023 23:23:12 GMT
VOLUME [/var/lib/kapacitor]
# Fri, 28 Apr 2023 23:23:12 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Fri, 28 Apr 2023 23:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Apr 2023 23:23:13 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562ec21068704bb8efd8a6db94153756f2ea649fc15b7a3d8c5ae495403deaff`  
		Last Modified: Fri, 28 Apr 2023 23:24:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d500101053a8592e41f90d59292cd74a1d55daea7ae9ae255f54f3c3b0bafa0`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 284.8 KB (284768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f632df2bffbd0c0aef5f148bd642609bbd3769c3a2f68af212c24569fe3059`  
		Last Modified: Fri, 28 Apr 2023 23:24:14 GMT  
		Size: 65.6 MB (65580141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe03849db0a97866932a7b703905538b0d9190b841dbc50e49d72d1840cf605`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f533d079920207448963e4c621b57d4b0faad5d7eabc65bf0171e777ec58e465`  
		Last Modified: Fri, 28 Apr 2023 23:24:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:3bc937bcd57a9eb476aa10e059ad331407fb7b7f787ccfcb577a941a2b405bed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:a4b03b00a2a79ddd0030143fe32c39ec8722b5eb6262eaa3d6e0278b62e73696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134578250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b48dbd6cef9c910481ef128df68501a0650fcbfcccb27106f370336706132bc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:26:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 16:09:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 16:09:31 GMT
ENV KAPACITOR_VERSION=1.6.6
# Wed, 03 May 2023 16:09:42 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 16:09:42 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 16:09:42 GMT
EXPOSE 9092
# Wed, 03 May 2023 16:09:42 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 16:09:42 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 16:09:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 16:09:42 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade6d81308cf88645476bddfaa8c5c2be767c77660b156a2bc5e740cd906431b`  
		Last Modified: Tue, 02 May 2023 23:43:33 GMT  
		Size: 7.1 MB (7123825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb507a78420a94908f02595d22f75332c5c8693df6cd0154f4e78a78ec2c12f2`  
		Last Modified: Wed, 03 May 2023 16:09:58 GMT  
		Size: 31.4 MB (31351810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e0cd46b31d30fa84eb9b19625e6f729983f718960a32c93c5fe9cc8bd2e50c`  
		Last Modified: Wed, 03 May 2023 16:10:23 GMT  
		Size: 65.7 MB (65672194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c120ea54647ec099a9b19129b4b91135f5ddb6073750d64a731feca9b2c2dfd8`  
		Last Modified: Wed, 03 May 2023 16:10:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7cee67f7a88d03d99a4e6bbbadfd77e7964a038d55adcdcbb3408582942834`  
		Last Modified: Wed, 03 May 2023 16:10:15 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:fd8637c1228eb50cf5f9a226f86d175e705572f38053eba3d4058eee650929bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (125995091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92d6c6598cff035de8737c99fe263363e373c50e88d82380cf960e953220d02`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Tue, 02 May 2023 23:56:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 14:10:10 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 03 May 2023 14:10:18 GMT
ENV KAPACITOR_VERSION=1.6.6
# Wed, 03 May 2023 14:10:24 GMT
RUN set -eux &&     ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in         amd64) ARCH='amd64';;         arm64) ARCH='arm64';;         *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     export GNUPGHOME="$(mktemp -d)" &&     echo "disable-ipv6" >> $GNUPGHOME/dirmngr.conf &&     gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -rf "$GNUPGHOME" &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpgconf --kill all &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 14:10:25 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 03 May 2023 14:10:25 GMT
EXPOSE 9092
# Wed, 03 May 2023 14:10:25 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 03 May 2023 14:10:25 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 03 May 2023 14:10:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 14:10:25 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1026f845342a6b9d1ce7fd9eafb77e2f1f29edebd77279101a8dbcf8c6d9dc1d`  
		Last Modified: Wed, 03 May 2023 00:15:25 GMT  
		Size: 7.1 MB (7065779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d123d3a8b02a77eaa4722bc4519550be04423f94bd1a64d9766c78b317e499`  
		Last Modified: Wed, 03 May 2023 14:10:36 GMT  
		Size: 28.9 MB (28872127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda45cfde5f7e38f5448246f9f11a613c4f44d625ba7d09c12190c77e3d64a2d`  
		Last Modified: Wed, 03 May 2023 14:10:50 GMT  
		Size: 61.7 MB (61669174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2f1193370470f52effdf853b25fe024dcb454fd638faf54c8205ecd57c3450`  
		Last Modified: Wed, 03 May 2023 14:10:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7bf8ddec5971b38e6b568b3e0c344e51318ca96c8955f2a7dadb0f3f689983`  
		Last Modified: Wed, 03 May 2023 14:10:44 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
