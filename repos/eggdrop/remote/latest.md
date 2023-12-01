## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:70dc745804b3f10e222df038fd2b0dbca9d03ea3e1c9ad4b8beaa5772aa43409
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
$ docker pull eggdrop@sha256:ffe6eb7e0bb3054579be5cc765a23ecadf04c22ddc3c98b86bd6f602fe3676e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11364123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac671ce6b36f2da35f2884ec0e94f5d8f2a5bebf30ccbf2e741a2b458ac51364`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:24 GMT
ADD file:cde69ed9ff455c9499e13b92a67b8722a1710401c31263561cf43c64193c3d80 in / 
# Thu, 30 Nov 2023 22:49:24 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:46:51 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 01 Dec 2023 00:46:51 GMT
RUN adduser -S eggdrop
# Fri, 01 Dec 2023 00:46:53 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 01 Dec 2023 00:46:55 GMT
RUN apk add --no-cache tcl bash openssl
# Fri, 01 Dec 2023 00:51:21 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 01 Dec 2023 00:51:21 GMT
ENV NICK=
# Fri, 01 Dec 2023 00:51:21 GMT
ENV SERVER=
# Fri, 01 Dec 2023 00:51:22 GMT
ENV LISTEN=3333
# Fri, 01 Dec 2023 00:51:22 GMT
ENV OWNER=
# Fri, 01 Dec 2023 00:51:22 GMT
ENV USERFILE=eggdrop.user
# Fri, 01 Dec 2023 00:51:22 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 01 Dec 2023 00:51:22 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 01 Dec 2023 00:51:22 GMT
EXPOSE 3333
# Fri, 01 Dec 2023 00:51:22 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Fri, 01 Dec 2023 00:51:22 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 01 Dec 2023 00:51:22 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 01 Dec 2023 00:51:22 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:b76d44755a1732ac572a54d4df4cfff9671b9466b719f4c80a81fd9397dbc3dc`  
		Last Modified: Thu, 30 Nov 2023 22:50:02 GMT  
		Size: 2.6 MB (2615844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f01547ebcbefe54eb1e1d4c830d6267f106a7d96af783934b9dfe604d127a1`  
		Last Modified: Fri, 01 Dec 2023 00:51:45 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268cff8e811083868c2ba79ef2660dbc1a22a7ff3b3ba9df49950ef850d6a8b2`  
		Last Modified: Fri, 01 Dec 2023 00:51:43 GMT  
		Size: 10.6 KB (10632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa31b831a5d4bdb2effafcdd0888f5027d97246ebf06d4f990d605e53b06b76`  
		Last Modified: Fri, 01 Dec 2023 00:51:44 GMT  
		Size: 2.7 MB (2679957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5e3021fd6f9ddcaa07b1d3647ef984cf1fb80038313bdab8b0e51557ba1ed3`  
		Last Modified: Fri, 01 Dec 2023 00:51:45 GMT  
		Size: 6.1 MB (6053881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2674305667c95e0fcf4c8478934599200b7e73b948e1effd8caf542c392b63`  
		Last Modified: Fri, 01 Dec 2023 00:51:43 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbdd6b20772743b6be30c0765e81a3fad39b675ab73dfa22def4df9ff3133e9`  
		Last Modified: Fri, 01 Dec 2023 00:51:43 GMT  
		Size: 698.0 B  
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
