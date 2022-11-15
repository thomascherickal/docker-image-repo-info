<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `chronograf`

-	[`chronograf:1.10`](#chronograf110)
-	[`chronograf:1.10-alpine`](#chronograf110-alpine)
-	[`chronograf:1.10.0`](#chronograf1100)
-	[`chronograf:1.10.0-alpine`](#chronograf1100-alpine)
-	[`chronograf:1.7`](#chronograf17)
-	[`chronograf:1.7-alpine`](#chronograf17-alpine)
-	[`chronograf:1.7.17`](#chronograf1717)
-	[`chronograf:1.7.17-alpine`](#chronograf1717-alpine)
-	[`chronograf:1.8`](#chronograf18)
-	[`chronograf:1.8-alpine`](#chronograf18-alpine)
-	[`chronograf:1.8.10`](#chronograf1810)
-	[`chronograf:1.8.10-alpine`](#chronograf1810-alpine)
-	[`chronograf:1.9`](#chronograf19)
-	[`chronograf:1.9-alpine`](#chronograf19-alpine)
-	[`chronograf:1.9.4`](#chronograf194)
-	[`chronograf:1.9.4-alpine`](#chronograf194-alpine)
-	[`chronograf:alpine`](#chronografalpine)
-	[`chronograf:latest`](#chronograflatest)

## `chronograf:1.10`

```console
$ docker pull chronograf@sha256:fe561e1c1ffcd6942f5eab576ae67a264d2d799c5ea6c286346ec5ad17fb0a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10` - linux; amd64

```console
$ docker pull chronograf@sha256:182a8673b2420f04ab87f1caa3af33ce02e3822b20d6d6e0b4e6c4488d9ae668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81253796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa22173565f1441d091a2598c9f0d6cfb4e8a20dd4eb3a948871712392b2c924`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:27:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:27:41 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 14:27:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:50 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:50 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:50 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:51 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751b5fd79a2622995a5a8b20a9af3c131589850ec66af68b835500727b5c2038`  
		Last Modified: Tue, 15 Nov 2022 14:28:29 GMT  
		Size: 5.2 MB (5228673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9face4f63fe02f5c2b7725633c53fcfb3d1541a99c4e263866e55d9b605381`  
		Last Modified: Tue, 15 Nov 2022 14:29:03 GMT  
		Size: 44.6 MB (44588098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f2dfb3de6573e67cc7fe09ca82024f2266210bf00f7ae44f5bb1360204d410`  
		Last Modified: Tue, 15 Nov 2022 14:28:56 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8a191c5aa7c44ee2cba3dd5a2a3711ad6f0886b8c88e074049bf3684fd13c`  
		Last Modified: Tue, 15 Nov 2022 14:28:57 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8099be4e85dd79d853fb43db76aac1ff1deb11c7b1861334d839d44ccd867dd6`  
		Last Modified: Tue, 15 Nov 2022 14:28:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:73faecaca432c3dba55288fb2f4bce07cdf8d16188a7fe8f07e6b06f4f639763
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73560455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21db32e9f8ab2a11ad052adbaeb03e3f031aa69ef241e4f6958c3b08cb41c80c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:13:04 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 12:13:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:13:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:13:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:13:14 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:13:15 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:13:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:13:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:13:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118439706100e2536364e0a7909c17a0e97502d09e6cef1f5fcf85371e6d767c`  
		Last Modified: Tue, 15 Nov 2022 12:14:07 GMT  
		Size: 4.5 MB (4494978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d881550c0f258caec8cb2e72bccef84e085b776435200a059d49847dff4783`  
		Last Modified: Tue, 15 Nov 2022 12:14:44 GMT  
		Size: 42.5 MB (42464891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cac2e60b326d356648abb3d6bfe415011f8bd66147b2d3ec1b3236f3055684f`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344219e1493f8d5d359b71e27b1ea1de083ab0ea6b505d3a8c03669762cc671a`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbb6a1869ce0007c21319ca79ce86193e1235cd80341ab1a4f207269de6ed61`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:b44cb4a7992a1595ca22e7e47f101b24f25adb3d3f5a7306b2f24db4743ed1b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77914437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8996f52c2544409e68fae4032f072e3460624039abeda9ebec5da5556987dc65`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:39 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 05:46:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:46 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:46 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1302dbefd893d577e12e191638448c1a51cbb0cb17a339f83b394823ff78b90`  
		Last Modified: Tue, 15 Nov 2022 05:47:14 GMT  
		Size: 5.2 MB (5211562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ad8c453bfced5539d3aa33b100006f0aad42b6d69b3df9b9ad69a22aa542c9`  
		Last Modified: Tue, 15 Nov 2022 05:47:50 GMT  
		Size: 42.6 MB (42617875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e940e47c5d89f9cc5fd42f636314aa1c09887dbeba64a2df7e30661a5f6ae5`  
		Last Modified: Tue, 15 Nov 2022 05:47:37 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a927b1e87b319deedf6236aff848b3c7e363b585b0be7af3cd6f2b8e00efcc`  
		Last Modified: Tue, 15 Nov 2022 05:47:36 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc864ced863464d1ace6e8f7c95ba2ea2f2b4d8f9aa2670624015d89611ff7`  
		Last Modified: Tue, 15 Nov 2022 05:47:37 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10-alpine`

```console
$ docker pull chronograf@sha256:c92d2e5d3aaed3d5abd3e21e85b3dd60e8169f7bf6699f473aed28eabff1d043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:de6c4148eeb1291ced92120697fad8332c74a726171672daf7c7b67e21d3850b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30311143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d58f859d1dc29bb2ee9f917635f6eb5621000d9d6619ec8ad4549203995550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:16:09 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Thu, 06 Oct 2022 20:16:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:17 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eea9d4a8a69cd5e2e5fca1b123ba2cd44364cf36b128c2fe59a5edf12221dfd`  
		Last Modified: Thu, 06 Oct 2022 20:17:26 GMT  
		Size: 27.2 MB (27174517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a685cca594b365e8c9e5d2a452959ac02b6fde12a79d898abf1a833a483707`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dba48a5545ef21547b2590458104e7bf680e4a5afbd1707de156d2d9420751`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ece5a9a06b7739faf864ebca0e4561819e3e331b928666a09e2c5bb2b9b2181`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.0`

```console
$ docker pull chronograf@sha256:fe561e1c1ffcd6942f5eab576ae67a264d2d799c5ea6c286346ec5ad17fb0a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.10.0` - linux; amd64

```console
$ docker pull chronograf@sha256:182a8673b2420f04ab87f1caa3af33ce02e3822b20d6d6e0b4e6c4488d9ae668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81253796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa22173565f1441d091a2598c9f0d6cfb4e8a20dd4eb3a948871712392b2c924`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:27:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:27:41 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 14:27:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:50 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:50 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:50 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:51 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751b5fd79a2622995a5a8b20a9af3c131589850ec66af68b835500727b5c2038`  
		Last Modified: Tue, 15 Nov 2022 14:28:29 GMT  
		Size: 5.2 MB (5228673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9face4f63fe02f5c2b7725633c53fcfb3d1541a99c4e263866e55d9b605381`  
		Last Modified: Tue, 15 Nov 2022 14:29:03 GMT  
		Size: 44.6 MB (44588098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f2dfb3de6573e67cc7fe09ca82024f2266210bf00f7ae44f5bb1360204d410`  
		Last Modified: Tue, 15 Nov 2022 14:28:56 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8a191c5aa7c44ee2cba3dd5a2a3711ad6f0886b8c88e074049bf3684fd13c`  
		Last Modified: Tue, 15 Nov 2022 14:28:57 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8099be4e85dd79d853fb43db76aac1ff1deb11c7b1861334d839d44ccd867dd6`  
		Last Modified: Tue, 15 Nov 2022 14:28:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.0` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:73faecaca432c3dba55288fb2f4bce07cdf8d16188a7fe8f07e6b06f4f639763
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73560455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21db32e9f8ab2a11ad052adbaeb03e3f031aa69ef241e4f6958c3b08cb41c80c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:13:04 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 12:13:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:13:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:13:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:13:14 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:13:15 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:13:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:13:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:13:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118439706100e2536364e0a7909c17a0e97502d09e6cef1f5fcf85371e6d767c`  
		Last Modified: Tue, 15 Nov 2022 12:14:07 GMT  
		Size: 4.5 MB (4494978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d881550c0f258caec8cb2e72bccef84e085b776435200a059d49847dff4783`  
		Last Modified: Tue, 15 Nov 2022 12:14:44 GMT  
		Size: 42.5 MB (42464891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cac2e60b326d356648abb3d6bfe415011f8bd66147b2d3ec1b3236f3055684f`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344219e1493f8d5d359b71e27b1ea1de083ab0ea6b505d3a8c03669762cc671a`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbb6a1869ce0007c21319ca79ce86193e1235cd80341ab1a4f207269de6ed61`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.10.0` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:b44cb4a7992a1595ca22e7e47f101b24f25adb3d3f5a7306b2f24db4743ed1b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77914437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8996f52c2544409e68fae4032f072e3460624039abeda9ebec5da5556987dc65`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:39 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 05:46:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:46 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:46 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1302dbefd893d577e12e191638448c1a51cbb0cb17a339f83b394823ff78b90`  
		Last Modified: Tue, 15 Nov 2022 05:47:14 GMT  
		Size: 5.2 MB (5211562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ad8c453bfced5539d3aa33b100006f0aad42b6d69b3df9b9ad69a22aa542c9`  
		Last Modified: Tue, 15 Nov 2022 05:47:50 GMT  
		Size: 42.6 MB (42617875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e940e47c5d89f9cc5fd42f636314aa1c09887dbeba64a2df7e30661a5f6ae5`  
		Last Modified: Tue, 15 Nov 2022 05:47:37 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a927b1e87b319deedf6236aff848b3c7e363b585b0be7af3cd6f2b8e00efcc`  
		Last Modified: Tue, 15 Nov 2022 05:47:36 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc864ced863464d1ace6e8f7c95ba2ea2f2b4d8f9aa2670624015d89611ff7`  
		Last Modified: Tue, 15 Nov 2022 05:47:37 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.10.0-alpine`

```console
$ docker pull chronograf@sha256:c92d2e5d3aaed3d5abd3e21e85b3dd60e8169f7bf6699f473aed28eabff1d043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.10.0-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:de6c4148eeb1291ced92120697fad8332c74a726171672daf7c7b67e21d3850b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30311143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d58f859d1dc29bb2ee9f917635f6eb5621000d9d6619ec8ad4549203995550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:16:09 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Thu, 06 Oct 2022 20:16:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:17 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eea9d4a8a69cd5e2e5fca1b123ba2cd44364cf36b128c2fe59a5edf12221dfd`  
		Last Modified: Thu, 06 Oct 2022 20:17:26 GMT  
		Size: 27.2 MB (27174517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a685cca594b365e8c9e5d2a452959ac02b6fde12a79d898abf1a833a483707`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dba48a5545ef21547b2590458104e7bf680e4a5afbd1707de156d2d9420751`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ece5a9a06b7739faf864ebca0e4561819e3e331b928666a09e2c5bb2b9b2181`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7`

```console
$ docker pull chronograf@sha256:a1fbb2d7e6d92d38ed7b9608f3f193d844ad1766e3252b497169916ea5c2519b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7` - linux; amd64

```console
$ docker pull chronograf@sha256:59ea180bd37bf26550cd23be3715d8dfd1c335daaabb63263b770a5f184c08d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70594849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2da7a7c322fc300eca2664e23d19bff16ed973aa0a131b938443837cc224dae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:26:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:26:53 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 15 Nov 2022 14:27:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:01 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:01 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:01 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:01 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0e73bf5f0310d44ba1dac2be2767468aff60744030ddc15eae8f19b7d933a7`  
		Last Modified: Tue, 15 Nov 2022 14:28:15 GMT  
		Size: 4.4 MB (4418930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce057e60ef898a6021adbb3f183a4a33efe9974f7f140e3d692913c6ec9bd4e`  
		Last Modified: Tue, 15 Nov 2022 14:28:19 GMT  
		Size: 34.7 MB (34738894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31138d5491b6a1596bcbc9d261fbe409d5eef185e4f3f67b821467e5dfa5e466`  
		Last Modified: Tue, 15 Nov 2022 14:28:14 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac1ce6716c26ca314f393e8df680d6094061fbb49e3402474b944d3375b6b19`  
		Last Modified: Tue, 15 Nov 2022 14:28:14 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859cd205b69af3863a994674296bf728f3e1862818d27b9db690de86a5111224`  
		Last Modified: Tue, 15 Nov 2022 14:28:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:94a975ac5f53b94a4b90bb79a70362ed79f63498eb5edf680e42172ca0fcbc4b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63419256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ca68f2d67ba8acc81660227085ac057bea36a81135318f8b0a3301e7828302`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:12:08 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 15 Nov 2022 12:12:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:12:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:12:18 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:12:18 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:12:18 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:12:19 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:12:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:12:19 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177030b100b97185289ce750be38c5366d62050c31319cdfa3dbc2e13fc86ed5`  
		Last Modified: Tue, 15 Nov 2022 12:13:50 GMT  
		Size: 3.7 MB (3720166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbea54e68eebe1f4bbb5559c1f113a9be57c728eae85d83a864f2a6beaa8d913`  
		Last Modified: Tue, 15 Nov 2022 12:13:55 GMT  
		Size: 33.1 MB (33098511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff844776136cb1f30f50cdd3284c5fe25da75420704bfdcf699408978b5d9d5`  
		Last Modified: Tue, 15 Nov 2022 12:13:50 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e0213395ab52fac4ebc24928389c6f30b30c930e28ac72bbba3a14c60539ab`  
		Last Modified: Tue, 15 Nov 2022 12:13:49 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecda22feb682035bb6a8a2ff8244e2328afae9a7d24272c6524dd8cce95323c`  
		Last Modified: Tue, 15 Nov 2022 12:13:49 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c6e568b43972f9ade0ad94e88b0bd818f6c343fba328a6bfbdc4e0453231cc23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67743791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02529227539c8b16a2624c48448dbc557865849cbe83e84001bc558e3e8eebbd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:02 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:02 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 15 Nov 2022 05:46:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:09 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9e78859fd890523b958e47ab9c84aab9c80a3f0c85ecbeeb671622efaa8038`  
		Last Modified: Tue, 15 Nov 2022 05:47:01 GMT  
		Size: 4.4 MB (4420057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb29255c97bb7f6e830b84cdf2e4e15d55a16fbe92351c0e10add035c8d142`  
		Last Modified: Tue, 15 Nov 2022 05:47:04 GMT  
		Size: 33.2 MB (33238741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851e593d6f92afc7fd4fa8d831f3fdce87f4ec6da37d3b222ecca3173da5b475`  
		Last Modified: Tue, 15 Nov 2022 05:47:01 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f5896feb481e5040ed5042c551a408aba92e2c8e9d9ca5af9728b25d2886c9`  
		Last Modified: Tue, 15 Nov 2022 05:47:01 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f771bd12698bc68827e9cdf602ef951b1bc7c3ace7ca37153ff8812bea50da`  
		Last Modified: Tue, 15 Nov 2022 05:47:01 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7-alpine`

```console
$ docker pull chronograf@sha256:9d26ac37c933bc166fe620ded24d156485d317e71f04c4eb2878c565b984849f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4b6a35a54e58b60f161d3f2f58aed998b7a0ae7074ca382fda7ec2ada7c2e902
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22693433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6af57497b0aa0aca47fc1ff15bd6c753ed5fa7230450329b86857ba4351cc0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:37 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 06 Oct 2022 20:15:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:15:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:15:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:15:42 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:15:43 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:15:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:15:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fda7c0dc93cbe974534daa33cf7bf0b94c5803f47fb7f8116f83829cc52a701`  
		Last Modified: Thu, 06 Oct 2022 20:16:44 GMT  
		Size: 19.6 MB (19556809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf26481c4767c4543af0f2684354471d9d92c1d3ff7e3a43f714669312ddb5`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 12.3 KB (12264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ba3ac2384cc84a067095232897c2f0e30822a778f2bc4d7136e30d336f9a7b`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cdc8000c1828cc4d9f01bcd32824b8ef240f8130b247937bfb0159e925f412`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17`

```console
$ docker pull chronograf@sha256:a1fbb2d7e6d92d38ed7b9608f3f193d844ad1766e3252b497169916ea5c2519b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.7.17` - linux; amd64

```console
$ docker pull chronograf@sha256:59ea180bd37bf26550cd23be3715d8dfd1c335daaabb63263b770a5f184c08d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70594849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2da7a7c322fc300eca2664e23d19bff16ed973aa0a131b938443837cc224dae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:26:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:26:53 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 15 Nov 2022 14:27:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:01 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:01 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:01 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:01 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:01 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:01 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0e73bf5f0310d44ba1dac2be2767468aff60744030ddc15eae8f19b7d933a7`  
		Last Modified: Tue, 15 Nov 2022 14:28:15 GMT  
		Size: 4.4 MB (4418930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce057e60ef898a6021adbb3f183a4a33efe9974f7f140e3d692913c6ec9bd4e`  
		Last Modified: Tue, 15 Nov 2022 14:28:19 GMT  
		Size: 34.7 MB (34738894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31138d5491b6a1596bcbc9d261fbe409d5eef185e4f3f67b821467e5dfa5e466`  
		Last Modified: Tue, 15 Nov 2022 14:28:14 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac1ce6716c26ca314f393e8df680d6094061fbb49e3402474b944d3375b6b19`  
		Last Modified: Tue, 15 Nov 2022 14:28:14 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859cd205b69af3863a994674296bf728f3e1862818d27b9db690de86a5111224`  
		Last Modified: Tue, 15 Nov 2022 14:28:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:94a975ac5f53b94a4b90bb79a70362ed79f63498eb5edf680e42172ca0fcbc4b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63419256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ca68f2d67ba8acc81660227085ac057bea36a81135318f8b0a3301e7828302`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:12:08 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 15 Nov 2022 12:12:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:12:18 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:12:18 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:12:18 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:12:18 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:12:19 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:12:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:12:19 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177030b100b97185289ce750be38c5366d62050c31319cdfa3dbc2e13fc86ed5`  
		Last Modified: Tue, 15 Nov 2022 12:13:50 GMT  
		Size: 3.7 MB (3720166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbea54e68eebe1f4bbb5559c1f113a9be57c728eae85d83a864f2a6beaa8d913`  
		Last Modified: Tue, 15 Nov 2022 12:13:55 GMT  
		Size: 33.1 MB (33098511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff844776136cb1f30f50cdd3284c5fe25da75420704bfdcf699408978b5d9d5`  
		Last Modified: Tue, 15 Nov 2022 12:13:50 GMT  
		Size: 12.2 KB (12244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e0213395ab52fac4ebc24928389c6f30b30c930e28ac72bbba3a14c60539ab`  
		Last Modified: Tue, 15 Nov 2022 12:13:49 GMT  
		Size: 11.9 KB (11902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecda22feb682035bb6a8a2ff8244e2328afae9a7d24272c6524dd8cce95323c`  
		Last Modified: Tue, 15 Nov 2022 12:13:49 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.7.17` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:c6e568b43972f9ade0ad94e88b0bd818f6c343fba328a6bfbdc4e0453231cc23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67743791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02529227539c8b16a2624c48448dbc557865849cbe83e84001bc558e3e8eebbd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:02 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:02 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Tue, 15 Nov 2022 05:46:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:09 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:09 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:09 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:09 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:09 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:09 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9e78859fd890523b958e47ab9c84aab9c80a3f0c85ecbeeb671622efaa8038`  
		Last Modified: Tue, 15 Nov 2022 05:47:01 GMT  
		Size: 4.4 MB (4420057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb29255c97bb7f6e830b84cdf2e4e15d55a16fbe92351c0e10add035c8d142`  
		Last Modified: Tue, 15 Nov 2022 05:47:04 GMT  
		Size: 33.2 MB (33238741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851e593d6f92afc7fd4fa8d831f3fdce87f4ec6da37d3b222ecca3173da5b475`  
		Last Modified: Tue, 15 Nov 2022 05:47:01 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f5896feb481e5040ed5042c551a408aba92e2c8e9d9ca5af9728b25d2886c9`  
		Last Modified: Tue, 15 Nov 2022 05:47:01 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f771bd12698bc68827e9cdf602ef951b1bc7c3ace7ca37153ff8812bea50da`  
		Last Modified: Tue, 15 Nov 2022 05:47:01 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.7.17-alpine`

```console
$ docker pull chronograf@sha256:9d26ac37c933bc166fe620ded24d156485d317e71f04c4eb2878c565b984849f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.7.17-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:4b6a35a54e58b60f161d3f2f58aed998b7a0ae7074ca382fda7ec2ada7c2e902
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22693433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6af57497b0aa0aca47fc1ff15bd6c753ed5fa7230450329b86857ba4351cc0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:37 GMT
ENV CHRONOGRAF_VERSION=1.7.17
# Thu, 06 Oct 2022 20:15:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:15:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:15:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:15:42 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:15:43 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:15:43 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:15:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:15:43 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fda7c0dc93cbe974534daa33cf7bf0b94c5803f47fb7f8116f83829cc52a701`  
		Last Modified: Thu, 06 Oct 2022 20:16:44 GMT  
		Size: 19.6 MB (19556809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf26481c4767c4543af0f2684354471d9d92c1d3ff7e3a43f714669312ddb5`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 12.3 KB (12264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ba3ac2384cc84a067095232897c2f0e30822a778f2bc4d7136e30d336f9a7b`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 11.9 KB (11896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cdc8000c1828cc4d9f01bcd32824b8ef240f8130b247937bfb0159e925f412`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8`

```console
$ docker pull chronograf@sha256:2f22e484652748b51a7b908e95c16c2f8e48a1907f808c16d1cfc15f44bb9eba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8` - linux; amd64

```console
$ docker pull chronograf@sha256:4f924db6bd71353420d9e63d1c3d2d278cd33e613058eca833f13717496bece4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71245327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975d1fc0de3aafa869e7bb79827089bae0015d487da22d00eb9eb33fff868747`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:27:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:27:16 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 15 Nov 2022 14:27:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:24 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:24 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751b5fd79a2622995a5a8b20a9af3c131589850ec66af68b835500727b5c2038`  
		Last Modified: Tue, 15 Nov 2022 14:28:29 GMT  
		Size: 5.2 MB (5228673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ed57aefa8a1c1a7100fe4bf31cd8e3833dd88ce2021b00c71ce406a4e9cc38`  
		Last Modified: Tue, 15 Nov 2022 14:28:33 GMT  
		Size: 34.6 MB (34579630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453bd95d385239f79120c31f442ac7ab332320fd5223bc518f7142a0ea2385c`  
		Last Modified: Tue, 15 Nov 2022 14:28:28 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c428d5b711424373cebead4a581c9ccc00d9817180fdd3322eda4ea065519bc`  
		Last Modified: Tue, 15 Nov 2022 14:28:28 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969ae715321431e37fdccc717a1f5ca380745adb425973ce7079ad342a739a5c`  
		Last Modified: Tue, 15 Nov 2022 14:28:28 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3b5efeb7c1e9f376b3c28e8352182fe9aebb4800f4f6a8fc6ce67167f9955af6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63846748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8cd76a025404584a748655fc86d27ae53298042135168ed5e8556bf6999bd99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:12:33 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 15 Nov 2022 12:12:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:12:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:12:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:12:42 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:12:42 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:12:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:12:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:12:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118439706100e2536364e0a7909c17a0e97502d09e6cef1f5fcf85371e6d767c`  
		Last Modified: Tue, 15 Nov 2022 12:14:07 GMT  
		Size: 4.5 MB (4494978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd146a4a2d5c4b9eea3f61157f6c7c1feb8b1cc6d1d67c6ccd8e0cfca9a26d9c`  
		Last Modified: Tue, 15 Nov 2022 12:14:11 GMT  
		Size: 32.8 MB (32751183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba21794bc71023249c2b28f99b3bd7cd3e10fdda5b77b3d14f90a6c18d87d81`  
		Last Modified: Tue, 15 Nov 2022 12:14:06 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845217b1945246a364bfa7a9fd1efd22ffccb1007bb440cf3f2a41abadb0ea08`  
		Last Modified: Tue, 15 Nov 2022 12:14:06 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bcf9aab11e751251160a5e2e75d1dbe44a2002e28edad2e164dd7fac66f166`  
		Last Modified: Tue, 15 Nov 2022 12:14:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:942f3ecd29268b1fa54498bd1bf9aa91bd81221e0bf7c93ebb1a4e14b0d55f41
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67941030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc97909991aed31be2e35023187568b4bf28306f06fa43061a4a8e5654d278f8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:19 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 15 Nov 2022 05:46:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:25 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:25 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:25 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1302dbefd893d577e12e191638448c1a51cbb0cb17a339f83b394823ff78b90`  
		Last Modified: Tue, 15 Nov 2022 05:47:14 GMT  
		Size: 5.2 MB (5211562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a214bb5fe6b0c7be060384c92ff1439cd9241bf9e15d62fcbd865a644ce68302`  
		Last Modified: Tue, 15 Nov 2022 05:47:16 GMT  
		Size: 32.6 MB (32644476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7999ac10c666760d9eba3c73503704c0bdddab1949daff8538407b99312085`  
		Last Modified: Tue, 15 Nov 2022 05:47:13 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9033aff8d463e57d06ff7d171a6e406f1552832eb786cc57e72e5962e082f2f`  
		Last Modified: Tue, 15 Nov 2022 05:47:13 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa20d8176d67d35181493ddc69cb2b8006bb1a7234328bd0035a79cc3de4d11d`  
		Last Modified: Tue, 15 Nov 2022 05:47:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8-alpine`

```console
$ docker pull chronograf@sha256:a430e7dd4d3f94b4b711a4000e847f59465fe1e3d7e9997d59800fc7a5da10cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:2d4ad97697ce5c225b6e38515e3ea3b543e28f102c45917f4239ecca0ebadda5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22340855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610057aef173c70f1c0a6ce869e16af679c0a1e65c669ac3b8eaba8d112a527a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:47 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 06 Oct 2022 20:15:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:15:53 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:15:53 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:15:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:15:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59d8c24f659459b77a60f9b6c97614166735dca2ae5a9254e7733b3382432fa`  
		Last Modified: Thu, 06 Oct 2022 20:16:58 GMT  
		Size: 19.2 MB (19204225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaef5e9f5e1eba8a7b3a73db5c4d6efe6ba62e72d3c1a86384494b5fc0b6bc3`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd6d1543ef965519e2d993c8db13568b477c3c72bae7b6023a2cde9350376d1`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f5df71d2bc59720fcde07d37a3c2f558595676b2519551f3efda4830e28abc`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10`

```console
$ docker pull chronograf@sha256:2f22e484652748b51a7b908e95c16c2f8e48a1907f808c16d1cfc15f44bb9eba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.8.10` - linux; amd64

```console
$ docker pull chronograf@sha256:4f924db6bd71353420d9e63d1c3d2d278cd33e613058eca833f13717496bece4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71245327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975d1fc0de3aafa869e7bb79827089bae0015d487da22d00eb9eb33fff868747`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:27:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:27:16 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 15 Nov 2022 14:27:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:24 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:24 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:24 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:24 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:24 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:24 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751b5fd79a2622995a5a8b20a9af3c131589850ec66af68b835500727b5c2038`  
		Last Modified: Tue, 15 Nov 2022 14:28:29 GMT  
		Size: 5.2 MB (5228673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ed57aefa8a1c1a7100fe4bf31cd8e3833dd88ce2021b00c71ce406a4e9cc38`  
		Last Modified: Tue, 15 Nov 2022 14:28:33 GMT  
		Size: 34.6 MB (34579630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453bd95d385239f79120c31f442ac7ab332320fd5223bc518f7142a0ea2385c`  
		Last Modified: Tue, 15 Nov 2022 14:28:28 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c428d5b711424373cebead4a581c9ccc00d9817180fdd3322eda4ea065519bc`  
		Last Modified: Tue, 15 Nov 2022 14:28:28 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969ae715321431e37fdccc717a1f5ca380745adb425973ce7079ad342a739a5c`  
		Last Modified: Tue, 15 Nov 2022 14:28:28 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:3b5efeb7c1e9f376b3c28e8352182fe9aebb4800f4f6a8fc6ce67167f9955af6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63846748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8cd76a025404584a748655fc86d27ae53298042135168ed5e8556bf6999bd99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:12:33 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 15 Nov 2022 12:12:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:12:42 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:12:42 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:12:42 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:12:42 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:12:42 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:12:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:12:42 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118439706100e2536364e0a7909c17a0e97502d09e6cef1f5fcf85371e6d767c`  
		Last Modified: Tue, 15 Nov 2022 12:14:07 GMT  
		Size: 4.5 MB (4494978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd146a4a2d5c4b9eea3f61157f6c7c1feb8b1cc6d1d67c6ccd8e0cfca9a26d9c`  
		Last Modified: Tue, 15 Nov 2022 12:14:11 GMT  
		Size: 32.8 MB (32751183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba21794bc71023249c2b28f99b3bd7cd3e10fdda5b77b3d14f90a6c18d87d81`  
		Last Modified: Tue, 15 Nov 2022 12:14:06 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845217b1945246a364bfa7a9fd1efd22ffccb1007bb440cf3f2a41abadb0ea08`  
		Last Modified: Tue, 15 Nov 2022 12:14:06 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bcf9aab11e751251160a5e2e75d1dbe44a2002e28edad2e164dd7fac66f166`  
		Last Modified: Tue, 15 Nov 2022 12:14:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.8.10` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:942f3ecd29268b1fa54498bd1bf9aa91bd81221e0bf7c93ebb1a4e14b0d55f41
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67941030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc97909991aed31be2e35023187568b4bf28306f06fa43061a4a8e5654d278f8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:19 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Tue, 15 Nov 2022 05:46:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:25 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:25 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:25 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:25 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:25 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:26 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1302dbefd893d577e12e191638448c1a51cbb0cb17a339f83b394823ff78b90`  
		Last Modified: Tue, 15 Nov 2022 05:47:14 GMT  
		Size: 5.2 MB (5211562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a214bb5fe6b0c7be060384c92ff1439cd9241bf9e15d62fcbd865a644ce68302`  
		Last Modified: Tue, 15 Nov 2022 05:47:16 GMT  
		Size: 32.6 MB (32644476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7999ac10c666760d9eba3c73503704c0bdddab1949daff8538407b99312085`  
		Last Modified: Tue, 15 Nov 2022 05:47:13 GMT  
		Size: 12.2 KB (12243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9033aff8d463e57d06ff7d171a6e406f1552832eb786cc57e72e5962e082f2f`  
		Last Modified: Tue, 15 Nov 2022 05:47:13 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa20d8176d67d35181493ddc69cb2b8006bb1a7234328bd0035a79cc3de4d11d`  
		Last Modified: Tue, 15 Nov 2022 05:47:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.8.10-alpine`

```console
$ docker pull chronograf@sha256:a430e7dd4d3f94b4b711a4000e847f59465fe1e3d7e9997d59800fc7a5da10cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.8.10-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:2d4ad97697ce5c225b6e38515e3ea3b543e28f102c45917f4239ecca0ebadda5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.3 MB (22340855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610057aef173c70f1c0a6ce869e16af679c0a1e65c669ac3b8eaba8d112a527a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:47 GMT
ENV CHRONOGRAF_VERSION=1.8.10
# Thu, 06 Oct 2022 20:15:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:15:53 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:15:53 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:15:53 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:15:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:15:53 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59d8c24f659459b77a60f9b6c97614166735dca2ae5a9254e7733b3382432fa`  
		Last Modified: Thu, 06 Oct 2022 20:16:58 GMT  
		Size: 19.2 MB (19204225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaef5e9f5e1eba8a7b3a73db5c4d6efe6ba62e72d3c1a86384494b5fc0b6bc3`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 12.3 KB (12267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd6d1543ef965519e2d993c8db13568b477c3c72bae7b6023a2cde9350376d1`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 11.9 KB (11899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f5df71d2bc59720fcde07d37a3c2f558595676b2519551f3efda4830e28abc`  
		Last Modified: Thu, 06 Oct 2022 20:16:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9`

```console
$ docker pull chronograf@sha256:e482a8d84f8af659a67e4ef5dc347b6301e075bfb824f505a7642fb244b5ebdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9` - linux; amd64

```console
$ docker pull chronograf@sha256:b49af1469c354b9f529435a83312066f9837691c4b88f020664366bd713f82a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71892894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8890e5c1cfa064b160fd5b875720d957ec81af5d24eeae4ea67c781dadf5dfc2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:27:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:27:30 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 15 Nov 2022 14:27:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:36 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:36 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:37 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:37 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:37 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751b5fd79a2622995a5a8b20a9af3c131589850ec66af68b835500727b5c2038`  
		Last Modified: Tue, 15 Nov 2022 14:28:29 GMT  
		Size: 5.2 MB (5228673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030adce06c6ae6ca4a1114a183be331fabbb0c3c6bcf1fb3b17cac078ec127e9`  
		Last Modified: Tue, 15 Nov 2022 14:28:47 GMT  
		Size: 35.2 MB (35227202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e0df53cc8d19b76e8479b0c7c99deb06b7ffeaeafba8838fb26856eb302b5f`  
		Last Modified: Tue, 15 Nov 2022 14:28:42 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d21543625abb6b0be61ac0b514dc8dd464a74c1dad259fe2c1dfcca6c97d859`  
		Last Modified: Tue, 15 Nov 2022 14:28:42 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c3e185ae694d96b5a773f544d425b73ba7678981269d79c544a96f07c01e8`  
		Last Modified: Tue, 15 Nov 2022 14:28:42 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:cdd196c8b3a6cc34a768345976abbb2018d92a336ed8bca91bb8867bea213c74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64622811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00cbd3dca78b0059c91ab58ddb53f8d5f11521db8636e789c107da33978b431`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:12:49 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 15 Nov 2022 12:12:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:12:57 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:12:57 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:12:57 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:12:58 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:12:58 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:12:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:12:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118439706100e2536364e0a7909c17a0e97502d09e6cef1f5fcf85371e6d767c`  
		Last Modified: Tue, 15 Nov 2022 12:14:07 GMT  
		Size: 4.5 MB (4494978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e70beea29ef80832cdaa40569e4de4e106daa27c77ca919a59e52187016fca`  
		Last Modified: Tue, 15 Nov 2022 12:14:26 GMT  
		Size: 33.5 MB (33527249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52869fba3c245b708f042f01f4fc135852566685fb0f37037f0a279f0ef98abd`  
		Last Modified: Tue, 15 Nov 2022 12:14:21 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8efbe2197e88ee557659fca0d2c70298ba0fc1120e4dcf1f2505a8bfb3858e`  
		Last Modified: Tue, 15 Nov 2022 12:14:21 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fbafdf4fac428c193e5803400db5f7f68514261143f39d9c2beab9773fb5c`  
		Last Modified: Tue, 15 Nov 2022 12:14:21 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:4720086058b39f51531c7a1f1e390f400e2d686f2cbda112fedaa0cd49db0065
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68692646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3833d0adf798e4ffc43eb99a66a240b199de07a0d5930d721518d275a6c57655`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:29 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 15 Nov 2022 05:46:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:35 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:35 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:35 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1302dbefd893d577e12e191638448c1a51cbb0cb17a339f83b394823ff78b90`  
		Last Modified: Tue, 15 Nov 2022 05:47:14 GMT  
		Size: 5.2 MB (5211562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c737275802976da3247149bc24cadf2535ecdb4dff87575e668bd2756daf98`  
		Last Modified: Tue, 15 Nov 2022 05:47:28 GMT  
		Size: 33.4 MB (33396084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c46d73b0ef28a4cd25c6d360e16468606fbaf7a53d697fe01f445bd22d202a8`  
		Last Modified: Tue, 15 Nov 2022 05:47:25 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e6e6f6f033ffeb3e52fee3ee5fd91099d5a9ffd96b85fb7a4f6e4f2a5bd7fd`  
		Last Modified: Tue, 15 Nov 2022 05:47:25 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96300bbf1e9048d62f02076975c7fa27d07d18dcafa1c84c0e235f88883c35d9`  
		Last Modified: Tue, 15 Nov 2022 05:47:25 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9-alpine`

```console
$ docker pull chronograf@sha256:22f17928ed0e686715e2b906f6e647ccc55c1e216dff1a563b76264f87f5392d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:d0b7ec6f54d4499c9a81a50fd7148b478b660fc8ded25155fb3a13baa4bf6239
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22808795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a3777d2e14c286895c264ba3580085a048c076a33a63ce90569c4ea6d7b2f98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:57 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 06 Oct 2022 20:16:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:04 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:04 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:04 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dfd580c937a95d72fb2af50a28c6814b4886872b951143883b0ffde4712c5f`  
		Last Modified: Thu, 06 Oct 2022 20:17:11 GMT  
		Size: 19.7 MB (19672168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e61e6634ea5e9aa1e5e15257ac4db9252543ec14ac7bd8989d98dca8f7b54f`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f00f1a43c212b770a42e5c7bc1563a4df034c07a36e2d6f937d26b1d907303e`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb73bba03a148277f19627c4b0811fb06e034afa29b8939eb47b20577a3537`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4`

```console
$ docker pull chronograf@sha256:e482a8d84f8af659a67e4ef5dc347b6301e075bfb824f505a7642fb244b5ebdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:1.9.4` - linux; amd64

```console
$ docker pull chronograf@sha256:b49af1469c354b9f529435a83312066f9837691c4b88f020664366bd713f82a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71892894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8890e5c1cfa064b160fd5b875720d957ec81af5d24eeae4ea67c781dadf5dfc2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:27:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:27:30 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 15 Nov 2022 14:27:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:36 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:36 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:36 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:37 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:37 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:37 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751b5fd79a2622995a5a8b20a9af3c131589850ec66af68b835500727b5c2038`  
		Last Modified: Tue, 15 Nov 2022 14:28:29 GMT  
		Size: 5.2 MB (5228673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030adce06c6ae6ca4a1114a183be331fabbb0c3c6bcf1fb3b17cac078ec127e9`  
		Last Modified: Tue, 15 Nov 2022 14:28:47 GMT  
		Size: 35.2 MB (35227202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e0df53cc8d19b76e8479b0c7c99deb06b7ffeaeafba8838fb26856eb302b5f`  
		Last Modified: Tue, 15 Nov 2022 14:28:42 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d21543625abb6b0be61ac0b514dc8dd464a74c1dad259fe2c1dfcca6c97d859`  
		Last Modified: Tue, 15 Nov 2022 14:28:42 GMT  
		Size: 11.9 KB (11903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c3e185ae694d96b5a773f544d425b73ba7678981269d79c544a96f07c01e8`  
		Last Modified: Tue, 15 Nov 2022 14:28:42 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:cdd196c8b3a6cc34a768345976abbb2018d92a336ed8bca91bb8867bea213c74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64622811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00cbd3dca78b0059c91ab58ddb53f8d5f11521db8636e789c107da33978b431`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:12:49 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 15 Nov 2022 12:12:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:12:57 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:12:57 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:12:57 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:12:58 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:12:58 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:12:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:12:58 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118439706100e2536364e0a7909c17a0e97502d09e6cef1f5fcf85371e6d767c`  
		Last Modified: Tue, 15 Nov 2022 12:14:07 GMT  
		Size: 4.5 MB (4494978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e70beea29ef80832cdaa40569e4de4e106daa27c77ca919a59e52187016fca`  
		Last Modified: Tue, 15 Nov 2022 12:14:26 GMT  
		Size: 33.5 MB (33527249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52869fba3c245b708f042f01f4fc135852566685fb0f37037f0a279f0ef98abd`  
		Last Modified: Tue, 15 Nov 2022 12:14:21 GMT  
		Size: 12.2 KB (12246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8efbe2197e88ee557659fca0d2c70298ba0fc1120e4dcf1f2505a8bfb3858e`  
		Last Modified: Tue, 15 Nov 2022 12:14:21 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fbafdf4fac428c193e5803400db5f7f68514261143f39d9c2beab9773fb5c`  
		Last Modified: Tue, 15 Nov 2022 12:14:21 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:1.9.4` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:4720086058b39f51531c7a1f1e390f400e2d686f2cbda112fedaa0cd49db0065
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68692646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3833d0adf798e4ffc43eb99a66a240b199de07a0d5930d721518d275a6c57655`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:29 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Tue, 15 Nov 2022 05:46:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:35 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:35 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:35 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:35 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:35 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:36 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1302dbefd893d577e12e191638448c1a51cbb0cb17a339f83b394823ff78b90`  
		Last Modified: Tue, 15 Nov 2022 05:47:14 GMT  
		Size: 5.2 MB (5211562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c737275802976da3247149bc24cadf2535ecdb4dff87575e668bd2756daf98`  
		Last Modified: Tue, 15 Nov 2022 05:47:28 GMT  
		Size: 33.4 MB (33396084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c46d73b0ef28a4cd25c6d360e16468606fbaf7a53d697fe01f445bd22d202a8`  
		Last Modified: Tue, 15 Nov 2022 05:47:25 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e6e6f6f033ffeb3e52fee3ee5fd91099d5a9ffd96b85fb7a4f6e4f2a5bd7fd`  
		Last Modified: Tue, 15 Nov 2022 05:47:25 GMT  
		Size: 11.9 KB (11908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96300bbf1e9048d62f02076975c7fa27d07d18dcafa1c84c0e235f88883c35d9`  
		Last Modified: Tue, 15 Nov 2022 05:47:25 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:1.9.4-alpine`

```console
$ docker pull chronograf@sha256:22f17928ed0e686715e2b906f6e647ccc55c1e216dff1a563b76264f87f5392d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:1.9.4-alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:d0b7ec6f54d4499c9a81a50fd7148b478b660fc8ded25155fb3a13baa4bf6239
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.8 MB (22808795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a3777d2e14c286895c264ba3580085a048c076a33a63ce90569c4ea6d7b2f98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:15:57 GMT
ENV CHRONOGRAF_VERSION=1.9.4
# Thu, 06 Oct 2022 20:16:03 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:03 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:03 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:04 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:04 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:04 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:04 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dfd580c937a95d72fb2af50a28c6814b4886872b951143883b0ffde4712c5f`  
		Last Modified: Thu, 06 Oct 2022 20:17:11 GMT  
		Size: 19.7 MB (19672168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e61e6634ea5e9aa1e5e15257ac4db9252543ec14ac7bd8989d98dca8f7b54f`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f00f1a43c212b770a42e5c7bc1563a4df034c07a36e2d6f937d26b1d907303e`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 11.9 KB (11898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb73bba03a148277f19627c4b0811fb06e034afa29b8939eb47b20577a3537`  
		Last Modified: Thu, 06 Oct 2022 20:17:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:alpine`

```console
$ docker pull chronograf@sha256:c92d2e5d3aaed3d5abd3e21e85b3dd60e8169f7bf6699f473aed28eabff1d043
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `chronograf:alpine` - linux; amd64

```console
$ docker pull chronograf@sha256:de6c4148eeb1291ced92120697fad8332c74a726171672daf7c7b67e21d3850b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30311143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d58f859d1dc29bb2ee9f917635f6eb5621000d9d6619ec8ad4549203995550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:15:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:15:37 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Thu, 06 Oct 2022 20:16:09 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Thu, 06 Oct 2022 20:16:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/chronograf/releases/chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz.asc chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf chronograf-${CHRONOGRAF_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/chronograf-*/chronograf.conf &&     chmod +x /usr/src/chronograf-*/* &&     cp -a /usr/src/chronograf-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 06 Oct 2022 20:16:17 GMT
EXPOSE 8888
# Thu, 06 Oct 2022 20:16:17 GMT
VOLUME [/var/lib/chronograf]
# Thu, 06 Oct 2022 20:16:17 GMT
COPY file:91fe01086b7984524af1eeb6657c6aea15ce5e169fd42a42e1ef2c54374d30a2 in /entrypoint.sh 
# Thu, 06 Oct 2022 20:16:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 20:16:17 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133509570f70da73b5369d8311a4269568dbea851313f10ea1b8cb1a2c4e2fe8`  
		Last Modified: Thu, 06 Oct 2022 20:16:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed07ae854e5b9e7d93d0c5eb8bbcfb2d6e5eddeb00720efe7b55766ce5bfbab`  
		Last Modified: Thu, 06 Oct 2022 20:16:41 GMT  
		Size: 284.6 KB (284583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eea9d4a8a69cd5e2e5fca1b123ba2cd44364cf36b128c2fe59a5edf12221dfd`  
		Last Modified: Thu, 06 Oct 2022 20:17:26 GMT  
		Size: 27.2 MB (27174517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a685cca594b365e8c9e5d2a452959ac02b6fde12a79d898abf1a833a483707`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 12.3 KB (12265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dba48a5545ef21547b2590458104e7bf680e4a5afbd1707de156d2d9420751`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 11.9 KB (11897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ece5a9a06b7739faf864ebca0e4561819e3e331b928666a09e2c5bb2b9b2181`  
		Last Modified: Thu, 06 Oct 2022 20:17:21 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `chronograf:latest`

```console
$ docker pull chronograf@sha256:fe561e1c1ffcd6942f5eab576ae67a264d2d799c5ea6c286346ec5ad17fb0a8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:182a8673b2420f04ab87f1caa3af33ce02e3822b20d6d6e0b4e6c4488d9ae668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81253796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa22173565f1441d091a2598c9f0d6cfb4e8a20dd4eb3a948871712392b2c924`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:27:16 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 14:27:41 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 14:27:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 14:27:50 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 14:27:50 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 14:27:50 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 14:27:50 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 14:27:51 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 14:27:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 14:27:51 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751b5fd79a2622995a5a8b20a9af3c131589850ec66af68b835500727b5c2038`  
		Last Modified: Tue, 15 Nov 2022 14:28:29 GMT  
		Size: 5.2 MB (5228673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9face4f63fe02f5c2b7725633c53fcfb3d1541a99c4e263866e55d9b605381`  
		Last Modified: Tue, 15 Nov 2022 14:29:03 GMT  
		Size: 44.6 MB (44588098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f2dfb3de6573e67cc7fe09ca82024f2266210bf00f7ae44f5bb1360204d410`  
		Last Modified: Tue, 15 Nov 2022 14:28:56 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8a191c5aa7c44ee2cba3dd5a2a3711ad6f0886b8c88e074049bf3684fd13c`  
		Last Modified: Tue, 15 Nov 2022 14:28:57 GMT  
		Size: 11.9 KB (11909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8099be4e85dd79d853fb43db76aac1ff1deb11c7b1861334d839d44ccd867dd6`  
		Last Modified: Tue, 15 Nov 2022 14:28:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:73faecaca432c3dba55288fb2f4bce07cdf8d16188a7fe8f07e6b06f4f639763
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73560455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21db32e9f8ab2a11ad052adbaeb03e3f031aa69ef241e4f6958c3b08cb41c80c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:12:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 12:13:04 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 12:13:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 12:13:14 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 12:13:14 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 12:13:14 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 12:13:15 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 12:13:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 12:13:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 12:13:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118439706100e2536364e0a7909c17a0e97502d09e6cef1f5fcf85371e6d767c`  
		Last Modified: Tue, 15 Nov 2022 12:14:07 GMT  
		Size: 4.5 MB (4494978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d881550c0f258caec8cb2e72bccef84e085b776435200a059d49847dff4783`  
		Last Modified: Tue, 15 Nov 2022 12:14:44 GMT  
		Size: 42.5 MB (42464891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cac2e60b326d356648abb3d6bfe415011f8bd66147b2d3ec1b3236f3055684f`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 12.2 KB (12247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344219e1493f8d5d359b71e27b1ea1de083ab0ea6b505d3a8c03669762cc671a`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 11.9 KB (11906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbb6a1869ce0007c21319ca79ce86193e1235cd80341ab1a4f207269de6ed61`  
		Last Modified: Tue, 15 Nov 2022 12:14:36 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:b44cb4a7992a1595ca22e7e47f101b24f25adb3d3f5a7306b2f24db4743ed1b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77914437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8996f52c2544409e68fae4032f072e3460624039abeda9ebec5da5556987dc65`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:46:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 15 Nov 2022 05:46:39 GMT
ENV CHRONOGRAF_VERSION=1.10.0
# Tue, 15 Nov 2022 05:46:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Tue, 15 Nov 2022 05:46:46 GMT
EXPOSE 8888
# Tue, 15 Nov 2022 05:46:46 GMT
VOLUME [/var/lib/chronograf]
# Tue, 15 Nov 2022 05:46:46 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Tue, 15 Nov 2022 05:46:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 15 Nov 2022 05:46:46 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1302dbefd893d577e12e191638448c1a51cbb0cb17a339f83b394823ff78b90`  
		Last Modified: Tue, 15 Nov 2022 05:47:14 GMT  
		Size: 5.2 MB (5211562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ad8c453bfced5539d3aa33b100006f0aad42b6d69b3df9b9ad69a22aa542c9`  
		Last Modified: Tue, 15 Nov 2022 05:47:50 GMT  
		Size: 42.6 MB (42617875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e940e47c5d89f9cc5fd42f636314aa1c09887dbeba64a2df7e30661a5f6ae5`  
		Last Modified: Tue, 15 Nov 2022 05:47:37 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a927b1e87b319deedf6236aff848b3c7e363b585b0be7af3cd6f2b8e00efcc`  
		Last Modified: Tue, 15 Nov 2022 05:47:36 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc864ced863464d1ace6e8f7c95ba2ea2f2b4d8f9aa2670624015d89611ff7`  
		Last Modified: Tue, 15 Nov 2022 05:47:37 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
