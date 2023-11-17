<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.5`](#eggdrop195)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:acde2b84d772dd00f1c03ed9b320803699bca9864cf0b1bfdd786b1274b91576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:cef44dbd708c4665b08a26e167e33a2967680666bf64b155bc4fd746e2318a6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13212395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66818451e0fcafd57cb96d68ac54b4bee7bb435564b0b8cafc43e9af4ef39691`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:21:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:21:04 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:21:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:21:06 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:24:59 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:25:00 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:25:00 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:25:00 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:25:00 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:25:00 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:25:00 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:25:00 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:25:01 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:25:01 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9153c6a700182d58d7b5ef3b1d6766db52fb8cffd5ebe0963370e3573d92bb45`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1be5449f4c5d26b81aa36d225e159f535d1bb13cc5fe6b7df20475cd7ed9a2b`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 10.9 KB (10942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d6b3b7c52d88578190c560710fcf48d1e168a89fa95c86bf4cea9cc6d5e690`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 4.2 MB (4243038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48379e358f27f6b31d1d26178f98a1d33a45c8a5a7dc8cf278da648b78adf2ac`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 6.1 MB (6146925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c90e0f2e200513380c1ef9a0c9369eef67c1ae9f04ab81ab67b4ad554add81e`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45e534423a160db620a625f83e51709d65eb47fa3b3e04927045e791805e357`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:57c4adf13ffef7f1a8cf8cc5acaa73946cf99529c865d9d8fa8ca1e5fac3965a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.6 MB (12604636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63a8d2f75f6ccc3d1cf344d3850999445179909742f340228283da3f16d2ae8`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:20 GMT
ADD file:321b24cc0fbd39caa2d7672a740d2cd2030ba99cab16f50c22db9955bd99350b in / 
# Mon, 07 Aug 2023 19:49:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:14:55 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:14:55 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:14:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:14:59 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:19:23 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:19:23 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:19:23 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:19:23 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:19:23 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:19:23 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:19:24 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:19:24 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:19:24 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:24 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:dffa980f71c953938bb194a457aa62e7f1885137331eef8bf7f9403c075f711c`  
		Last Modified: Mon, 07 Aug 2023 19:50:02 GMT  
		Size: 2.6 MB (2615553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b1608bea81ea60da0af667395e1c9d851be957bc6b1b4aa83b019a935c39d`  
		Last Modified: Sat, 21 Oct 2023 00:19:53 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d09e594aa48afc0a260df361facea90490867e9ec7baf12cd5faf0bef5d5955`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 10.6 KB (10640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cf033c4f989b00eb21778c77ae29710d13ab21e23094014cd74e410f0581cb`  
		Last Modified: Sat, 21 Oct 2023 00:19:52 GMT  
		Size: 3.9 MB (3920769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79a74fc6ac122fa29c48b9dbbbd76cf03de6a2a40d2f45970f5707baa358a7e`  
		Last Modified: Sat, 21 Oct 2023 00:19:52 GMT  
		Size: 6.1 MB (6053869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f877faed38f83d67d39f618617979922b02d1c4c7113feab8aa2f9348049e`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0066c35338b1975c76283682552537b92745a0b401193788c539cc863097ce9b`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:335d21f489281a90f8a50a6f7f9a87283a422e23c542893d1bdf1e4818d372fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (13044787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fac6512ce7508372ca55224d51e7ab610113dc08365fc6fd578a2ce17e907c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:30:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:30:23 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:30:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:30:26 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:34:06 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:34:06 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:34:06 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:34:07 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:34:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:34:07 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:34:07 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:34:07 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:34:07 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:34:07 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad45b36f18442ad26119b056504d92c7b9f62e328d40dfecc5b5cdada43d1b35`  
		Last Modified: Sat, 21 Oct 2023 00:34:34 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49388bb25b5f8ad759e0ad07f81cfde9d5582b983756e8755ca4a1767290cc27`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 10.8 KB (10753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da892d14d3f8723317aa360580e60ca34ede78811ab966eadaea3c2de639ee7d`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 4.1 MB (4134986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de50d5743266f6ac8088988db84ab43740c6b3132eedca57ede0934c826f02a`  
		Last Modified: Sat, 21 Oct 2023 00:34:33 GMT  
		Size: 6.2 MB (6187219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cb9c312acb1724d1054fb73e7b8b73415780d7fbac166f8065a010671b21f2`  
		Last Modified: Sat, 21 Oct 2023 00:34:31 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda22d55605db31fb6a4ebe445c1a75a0dbedefdbe7eab587cb33964630a46f`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.5`

```console
$ docker pull eggdrop@sha256:acde2b84d772dd00f1c03ed9b320803699bca9864cf0b1bfdd786b1274b91576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9.5` - linux; amd64

```console
$ docker pull eggdrop@sha256:cef44dbd708c4665b08a26e167e33a2967680666bf64b155bc4fd746e2318a6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13212395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66818451e0fcafd57cb96d68ac54b4bee7bb435564b0b8cafc43e9af4ef39691`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:21:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:21:04 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:21:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:21:06 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:24:59 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:25:00 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:25:00 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:25:00 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:25:00 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:25:00 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:25:00 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:25:00 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:25:01 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:25:01 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9153c6a700182d58d7b5ef3b1d6766db52fb8cffd5ebe0963370e3573d92bb45`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1be5449f4c5d26b81aa36d225e159f535d1bb13cc5fe6b7df20475cd7ed9a2b`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 10.9 KB (10942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d6b3b7c52d88578190c560710fcf48d1e168a89fa95c86bf4cea9cc6d5e690`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 4.2 MB (4243038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48379e358f27f6b31d1d26178f98a1d33a45c8a5a7dc8cf278da648b78adf2ac`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 6.1 MB (6146925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c90e0f2e200513380c1ef9a0c9369eef67c1ae9f04ab81ab67b4ad554add81e`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45e534423a160db620a625f83e51709d65eb47fa3b3e04927045e791805e357`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.5` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:57c4adf13ffef7f1a8cf8cc5acaa73946cf99529c865d9d8fa8ca1e5fac3965a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.6 MB (12604636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63a8d2f75f6ccc3d1cf344d3850999445179909742f340228283da3f16d2ae8`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:20 GMT
ADD file:321b24cc0fbd39caa2d7672a740d2cd2030ba99cab16f50c22db9955bd99350b in / 
# Mon, 07 Aug 2023 19:49:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:14:55 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:14:55 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:14:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:14:59 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:19:23 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:19:23 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:19:23 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:19:23 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:19:23 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:19:23 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:19:24 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:19:24 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:19:24 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:24 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:dffa980f71c953938bb194a457aa62e7f1885137331eef8bf7f9403c075f711c`  
		Last Modified: Mon, 07 Aug 2023 19:50:02 GMT  
		Size: 2.6 MB (2615553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b1608bea81ea60da0af667395e1c9d851be957bc6b1b4aa83b019a935c39d`  
		Last Modified: Sat, 21 Oct 2023 00:19:53 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d09e594aa48afc0a260df361facea90490867e9ec7baf12cd5faf0bef5d5955`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 10.6 KB (10640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cf033c4f989b00eb21778c77ae29710d13ab21e23094014cd74e410f0581cb`  
		Last Modified: Sat, 21 Oct 2023 00:19:52 GMT  
		Size: 3.9 MB (3920769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79a74fc6ac122fa29c48b9dbbbd76cf03de6a2a40d2f45970f5707baa358a7e`  
		Last Modified: Sat, 21 Oct 2023 00:19:52 GMT  
		Size: 6.1 MB (6053869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f877faed38f83d67d39f618617979922b02d1c4c7113feab8aa2f9348049e`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0066c35338b1975c76283682552537b92745a0b401193788c539cc863097ce9b`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.5` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:335d21f489281a90f8a50a6f7f9a87283a422e23c542893d1bdf1e4818d372fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (13044787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fac6512ce7508372ca55224d51e7ab610113dc08365fc6fd578a2ce17e907c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:30:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:30:23 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:30:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:30:26 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:34:06 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:34:06 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:34:06 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:34:07 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:34:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:34:07 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:34:07 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:34:07 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:34:07 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:34:07 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad45b36f18442ad26119b056504d92c7b9f62e328d40dfecc5b5cdada43d1b35`  
		Last Modified: Sat, 21 Oct 2023 00:34:34 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49388bb25b5f8ad759e0ad07f81cfde9d5582b983756e8755ca4a1767290cc27`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 10.8 KB (10753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da892d14d3f8723317aa360580e60ca34ede78811ab966eadaea3c2de639ee7d`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 4.1 MB (4134986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de50d5743266f6ac8088988db84ab43740c6b3132eedca57ede0934c826f02a`  
		Last Modified: Sat, 21 Oct 2023 00:34:33 GMT  
		Size: 6.2 MB (6187219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cb9c312acb1724d1054fb73e7b8b73415780d7fbac166f8065a010671b21f2`  
		Last Modified: Sat, 21 Oct 2023 00:34:31 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda22d55605db31fb6a4ebe445c1a75a0dbedefdbe7eab587cb33964630a46f`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:afe2edc84220f5db578e0dcc1349e624e36d9080a5343854dd9dcadd7ecf2a67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:9ec6b149a789433e2df240dce0dc83a36c33c82d50361683f7b1d0145331342a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.2 MB (18181286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4df521af73130bbe77b03bd8ecc6b8a34b79233f59eb491c1eadc2f4a50df0a`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:09 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:17:10 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:17:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:17:11 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Sat, 21 Oct 2023 00:17:11 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Sat, 21 Oct 2023 00:17:12 GMT
RUN apk --update add --no-cache bash openssl
# Sat, 21 Oct 2023 00:20:47 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:20:47 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:20:47 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:20:47 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:20:48 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:20:48 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:20:48 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:20:48 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:20:48 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:20:48 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:20:48 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:20:48 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:20:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097e7c90940c1ad08f4c14384b6e2b7bab2641e3962c1d08ea52eed9ae3cd5a`  
		Last Modified: Sat, 21 Oct 2023 00:25:21 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6848297e98706c32911ba7521bbbcb939e30b344e80d82a4c23ae786c4bce2c`  
		Last Modified: Sat, 21 Oct 2023 00:25:19 GMT  
		Size: 11.0 KB (10989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a7878a3e855d542a57210de1c56489094335eee11c07130b0fb1c43d9382d1`  
		Last Modified: Sat, 21 Oct 2023 00:25:19 GMT  
		Size: 3.3 MB (3252168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c554af8b3fe3416653bd54e0be76715af3815378bc526f99d99db471dcc56eab`  
		Last Modified: Sat, 21 Oct 2023 00:25:21 GMT  
		Size: 11.5 MB (11535291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcad910f3e97b3929931557c9fc1dd692de3dc7a35634dae4b16a1dcd47ad663`  
		Last Modified: Sat, 21 Oct 2023 00:25:19 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd80a7788f9c59b9fbbfe008475855d8ea16bf7def77b49ffcd90b07b9de35ca`  
		Last Modified: Sat, 21 Oct 2023 00:25:19 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:7ec24e9f4e60c69e368d49d2d118598683c4ce03b7f6b396f9764045daa8db22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17464976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c23cbe7f13a59d0657331d9ef3c321afc9e4a3ee006220b1642ad98dd1d19a6`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 00:49:16 GMT
LABEL org.opencontainers.image.authors=Geo Van O <geo@eggheads.org> org.opencontainers.image.url=https://www.eggheads.org
# Fri, 17 Nov 2023 00:49:17 GMT
RUN addgroup -S -g 3333 eggdrop     && adduser -S -u 3333 eggdrop eggdrop
# Fri, 17 Nov 2023 00:49:18 GMT
RUN apk add --no-cache 'su-exec>=0.2' bash openssl
# Fri, 17 Nov 2023 00:49:18 GMT
ENV EGGDROP_SHA256=a155625d2ac3a0673e69c9d0149293910583c1623cd1f90f38ad2bcba7b2b766
# Fri, 17 Nov 2023 00:49:19 GMT
ENV EGGDROP_COMMIT=322bddbd102d58cdb00864a3a335b086beaf042c
# Fri, 17 Nov 2023 00:51:31 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz --progress=dot:giga   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && nproc="$(nproc)"     && make -j"$nproc"     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && nproc="$(nproc)"     && make -j"$nproc"     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del --no-network egg-deps
# Fri, 17 Nov 2023 00:51:31 GMT
ENV NICK=
# Fri, 17 Nov 2023 00:51:31 GMT
ENV SERVER=
# Fri, 17 Nov 2023 00:51:31 GMT
ENV LISTEN=3333
# Fri, 17 Nov 2023 00:51:31 GMT
ENV USERFILE=eggdrop.user
# Fri, 17 Nov 2023 00:51:32 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 17 Nov 2023 00:51:32 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 17 Nov 2023 00:51:32 GMT
EXPOSE 3333
# Fri, 17 Nov 2023 00:51:32 GMT
COPY file:15b1df22891b2d819093301ed85a114b9e76e06ecf7eba8f403edb7908e4aebf in ./ 
# Fri, 17 Nov 2023 00:51:32 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in ./scripts/ 
# Fri, 17 Nov 2023 00:51:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 17 Nov 2023 00:51:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335fc6f78cbd562d8f9766b3257ac3d9b37fa428d12b64f5070920d39939eae0`  
		Last Modified: Fri, 17 Nov 2023 00:51:47 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861d3f8e3ba7e46d7b9ed9155c9a3fe18596e62335e22629aeef6ca4ba5e9021`  
		Last Modified: Fri, 17 Nov 2023 00:51:47 GMT  
		Size: 2.9 MB (2910069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a088eea7dc41afcb28fdefb3e171a8cd00c1fb63027a8a0a94ebb8d13e7dafc`  
		Last Modified: Fri, 17 Nov 2023 00:51:49 GMT  
		Size: 11.4 MB (11438170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576576d87dc427bcb07cbd63374bca0e5cae39bea4b2c10322dc45770ea62014`  
		Last Modified: Fri, 17 Nov 2023 00:51:47 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98259cceccb04b799758c7a457ef8f75825469cd4925e40995c3d32bca9b45b`  
		Last Modified: Fri, 17 Nov 2023 00:51:47 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:2b51503441c8d0ad8c293063e01ee3c6f71ecf9378d9ecd196e113aecdaa7519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (18014357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c036cf0a7b8624cbbafb8927c59054c637141b2798495b982c2dc35e1d348eb9`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 00:44:19 GMT
LABEL org.opencontainers.image.authors=Geo Van O <geo@eggheads.org> org.opencontainers.image.url=https://www.eggheads.org
# Fri, 17 Nov 2023 00:44:20 GMT
RUN addgroup -S -g 3333 eggdrop     && adduser -S -u 3333 eggdrop eggdrop
# Fri, 17 Nov 2023 00:44:21 GMT
RUN apk add --no-cache 'su-exec>=0.2' bash openssl
# Fri, 17 Nov 2023 00:44:21 GMT
ENV EGGDROP_SHA256=a155625d2ac3a0673e69c9d0149293910583c1623cd1f90f38ad2bcba7b2b766
# Fri, 17 Nov 2023 00:44:21 GMT
ENV EGGDROP_COMMIT=322bddbd102d58cdb00864a3a335b086beaf042c
# Fri, 17 Nov 2023 00:46:09 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz --progress=dot:giga   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && nproc="$(nproc)"     && make -j"$nproc"     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && nproc="$(nproc)"     && make -j"$nproc"     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del --no-network egg-deps
# Fri, 17 Nov 2023 00:46:09 GMT
ENV NICK=
# Fri, 17 Nov 2023 00:46:09 GMT
ENV SERVER=
# Fri, 17 Nov 2023 00:46:09 GMT
ENV LISTEN=3333
# Fri, 17 Nov 2023 00:46:09 GMT
ENV USERFILE=eggdrop.user
# Fri, 17 Nov 2023 00:46:10 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 17 Nov 2023 00:46:10 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 17 Nov 2023 00:46:10 GMT
EXPOSE 3333
# Fri, 17 Nov 2023 00:46:10 GMT
COPY file:15b1df22891b2d819093301ed85a114b9e76e06ecf7eba8f403edb7908e4aebf in ./ 
# Fri, 17 Nov 2023 00:46:10 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in ./scripts/ 
# Fri, 17 Nov 2023 00:46:10 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 17 Nov 2023 00:46:10 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778a29448c85f5349db5c2a8c91e09bb24415f8c010133b0976a97ae37a40256`  
		Last Modified: Fri, 17 Nov 2023 00:46:20 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbe65f838346d33f66aab8d53809a78314c0e63cafb944226af3d5b9e1acd46`  
		Last Modified: Fri, 17 Nov 2023 00:46:21 GMT  
		Size: 3.1 MB (3135693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1044c67968016b714c1417c534fae5525be432f8be37e1aa22528fc52937a96`  
		Last Modified: Fri, 17 Nov 2023 00:46:22 GMT  
		Size: 11.6 MB (11616090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f867e3dbd8ae6a6a2799e4e63e5eac1eb529cd7996efac37386069f76071d5e`  
		Last Modified: Fri, 17 Nov 2023 00:46:20 GMT  
		Size: 1.9 KB (1950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8332e40d2e076a34ba7e23d9aa4f6fb509a4396302ddd7c197fa95fe09a145`  
		Last Modified: Fri, 17 Nov 2023 00:46:20 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:acde2b84d772dd00f1c03ed9b320803699bca9864cf0b1bfdd786b1274b91576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:cef44dbd708c4665b08a26e167e33a2967680666bf64b155bc4fd746e2318a6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13212395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66818451e0fcafd57cb96d68ac54b4bee7bb435564b0b8cafc43e9af4ef39691`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:21:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:21:04 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:21:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:21:06 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:24:59 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:25:00 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:25:00 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:25:00 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:25:00 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:25:00 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:25:00 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:25:00 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:25:01 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:25:01 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9153c6a700182d58d7b5ef3b1d6766db52fb8cffd5ebe0963370e3573d92bb45`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1be5449f4c5d26b81aa36d225e159f535d1bb13cc5fe6b7df20475cd7ed9a2b`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 10.9 KB (10942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d6b3b7c52d88578190c560710fcf48d1e168a89fa95c86bf4cea9cc6d5e690`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 4.2 MB (4243038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48379e358f27f6b31d1d26178f98a1d33a45c8a5a7dc8cf278da648b78adf2ac`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 6.1 MB (6146925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c90e0f2e200513380c1ef9a0c9369eef67c1ae9f04ab81ab67b4ad554add81e`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45e534423a160db620a625f83e51709d65eb47fa3b3e04927045e791805e357`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:57c4adf13ffef7f1a8cf8cc5acaa73946cf99529c865d9d8fa8ca1e5fac3965a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.6 MB (12604636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63a8d2f75f6ccc3d1cf344d3850999445179909742f340228283da3f16d2ae8`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:20 GMT
ADD file:321b24cc0fbd39caa2d7672a740d2cd2030ba99cab16f50c22db9955bd99350b in / 
# Mon, 07 Aug 2023 19:49:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:14:55 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:14:55 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:14:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:14:59 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:19:23 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:19:23 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:19:23 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:19:23 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:19:23 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:19:23 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:19:24 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:19:24 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:19:24 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:24 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:dffa980f71c953938bb194a457aa62e7f1885137331eef8bf7f9403c075f711c`  
		Last Modified: Mon, 07 Aug 2023 19:50:02 GMT  
		Size: 2.6 MB (2615553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b1608bea81ea60da0af667395e1c9d851be957bc6b1b4aa83b019a935c39d`  
		Last Modified: Sat, 21 Oct 2023 00:19:53 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d09e594aa48afc0a260df361facea90490867e9ec7baf12cd5faf0bef5d5955`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 10.6 KB (10640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cf033c4f989b00eb21778c77ae29710d13ab21e23094014cd74e410f0581cb`  
		Last Modified: Sat, 21 Oct 2023 00:19:52 GMT  
		Size: 3.9 MB (3920769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79a74fc6ac122fa29c48b9dbbbd76cf03de6a2a40d2f45970f5707baa358a7e`  
		Last Modified: Sat, 21 Oct 2023 00:19:52 GMT  
		Size: 6.1 MB (6053869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f877faed38f83d67d39f618617979922b02d1c4c7113feab8aa2f9348049e`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0066c35338b1975c76283682552537b92745a0b401193788c539cc863097ce9b`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:335d21f489281a90f8a50a6f7f9a87283a422e23c542893d1bdf1e4818d372fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (13044787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fac6512ce7508372ca55224d51e7ab610113dc08365fc6fd578a2ce17e907c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:30:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:30:23 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:30:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:30:26 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:34:06 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:34:06 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:34:06 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:34:07 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:34:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:34:07 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:34:07 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:34:07 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:34:07 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:34:07 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad45b36f18442ad26119b056504d92c7b9f62e328d40dfecc5b5cdada43d1b35`  
		Last Modified: Sat, 21 Oct 2023 00:34:34 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49388bb25b5f8ad759e0ad07f81cfde9d5582b983756e8755ca4a1767290cc27`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 10.8 KB (10753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da892d14d3f8723317aa360580e60ca34ede78811ab966eadaea3c2de639ee7d`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 4.1 MB (4134986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de50d5743266f6ac8088988db84ab43740c6b3132eedca57ede0934c826f02a`  
		Last Modified: Sat, 21 Oct 2023 00:34:33 GMT  
		Size: 6.2 MB (6187219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cb9c312acb1724d1054fb73e7b8b73415780d7fbac166f8065a010671b21f2`  
		Last Modified: Sat, 21 Oct 2023 00:34:31 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda22d55605db31fb6a4ebe445c1a75a0dbedefdbe7eab587cb33964630a46f`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:acde2b84d772dd00f1c03ed9b320803699bca9864cf0b1bfdd786b1274b91576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:cef44dbd708c4665b08a26e167e33a2967680666bf64b155bc4fd746e2318a6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13212395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66818451e0fcafd57cb96d68ac54b4bee7bb435564b0b8cafc43e9af4ef39691`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:21:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:21:04 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:21:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:21:06 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:24:59 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:25:00 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:25:00 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:25:00 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:25:00 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:25:00 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:25:00 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:25:00 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:25:00 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:25:01 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:25:01 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9153c6a700182d58d7b5ef3b1d6766db52fb8cffd5ebe0963370e3573d92bb45`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1be5449f4c5d26b81aa36d225e159f535d1bb13cc5fe6b7df20475cd7ed9a2b`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 10.9 KB (10942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d6b3b7c52d88578190c560710fcf48d1e168a89fa95c86bf4cea9cc6d5e690`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 4.2 MB (4243038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48379e358f27f6b31d1d26178f98a1d33a45c8a5a7dc8cf278da648b78adf2ac`  
		Last Modified: Sat, 21 Oct 2023 00:25:28 GMT  
		Size: 6.1 MB (6146925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c90e0f2e200513380c1ef9a0c9369eef67c1ae9f04ab81ab67b4ad554add81e`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45e534423a160db620a625f83e51709d65eb47fa3b3e04927045e791805e357`  
		Last Modified: Sat, 21 Oct 2023 00:25:27 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:57c4adf13ffef7f1a8cf8cc5acaa73946cf99529c865d9d8fa8ca1e5fac3965a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.6 MB (12604636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63a8d2f75f6ccc3d1cf344d3850999445179909742f340228283da3f16d2ae8`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:20 GMT
ADD file:321b24cc0fbd39caa2d7672a740d2cd2030ba99cab16f50c22db9955bd99350b in / 
# Mon, 07 Aug 2023 19:49:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:14:55 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:14:55 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:14:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:14:59 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:19:23 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:19:23 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:19:23 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:19:23 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:19:23 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:19:23 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:19:23 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:19:24 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:19:24 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:19:24 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:24 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:dffa980f71c953938bb194a457aa62e7f1885137331eef8bf7f9403c075f711c`  
		Last Modified: Mon, 07 Aug 2023 19:50:02 GMT  
		Size: 2.6 MB (2615553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b1608bea81ea60da0af667395e1c9d851be957bc6b1b4aa83b019a935c39d`  
		Last Modified: Sat, 21 Oct 2023 00:19:53 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d09e594aa48afc0a260df361facea90490867e9ec7baf12cd5faf0bef5d5955`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 10.6 KB (10640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cf033c4f989b00eb21778c77ae29710d13ab21e23094014cd74e410f0581cb`  
		Last Modified: Sat, 21 Oct 2023 00:19:52 GMT  
		Size: 3.9 MB (3920769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79a74fc6ac122fa29c48b9dbbbd76cf03de6a2a40d2f45970f5707baa358a7e`  
		Last Modified: Sat, 21 Oct 2023 00:19:52 GMT  
		Size: 6.1 MB (6053869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848f877faed38f83d67d39f618617979922b02d1c4c7113feab8aa2f9348049e`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0066c35338b1975c76283682552537b92745a0b401193788c539cc863097ce9b`  
		Last Modified: Sat, 21 Oct 2023 00:19:51 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:335d21f489281a90f8a50a6f7f9a87283a422e23c542893d1bdf1e4818d372fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (13044787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fac6512ce7508372ca55224d51e7ab610113dc08365fc6fd578a2ce17e907c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:30:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:30:23 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:30:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:30:26 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 21 Oct 2023 00:34:06 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:34:06 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:34:06 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:34:06 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:34:07 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:34:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:34:07 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:34:07 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:34:07 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:34:07 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:34:07 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad45b36f18442ad26119b056504d92c7b9f62e328d40dfecc5b5cdada43d1b35`  
		Last Modified: Sat, 21 Oct 2023 00:34:34 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49388bb25b5f8ad759e0ad07f81cfde9d5582b983756e8755ca4a1767290cc27`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 10.8 KB (10753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da892d14d3f8723317aa360580e60ca34ede78811ab966eadaea3c2de639ee7d`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 4.1 MB (4134986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de50d5743266f6ac8088988db84ab43740c6b3132eedca57ede0934c826f02a`  
		Last Modified: Sat, 21 Oct 2023 00:34:33 GMT  
		Size: 6.2 MB (6187219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cb9c312acb1724d1054fb73e7b8b73415780d7fbac166f8065a010671b21f2`  
		Last Modified: Sat, 21 Oct 2023 00:34:31 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bda22d55605db31fb6a4ebe445c1a75a0dbedefdbe7eab587cb33964630a46f`  
		Last Modified: Sat, 21 Oct 2023 00:34:32 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
