## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:0f4d4ef7c9dcd201df2ca34005bd54c03c8e251883d5d110cc1382b126d68119
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:86b82bcbc18e3d56b832d60f0f242f07ea8131f12df1273232d23be7f5298ceb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14619050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:289b31aa30810d9f17fb7629fa43c6be80532051b8daddb882ccf7b2f91eb278`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:47:36 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 11 Feb 2023 07:47:37 GMT
RUN adduser -S eggdrop
# Sat, 11 Feb 2023 07:47:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 11 Feb 2023 07:47:38 GMT
ENV EGGDROP_SHA256=caafc1ad001e2e77793dca37998cb94d88efadb4ec9c3de44c1004b04f15aa6e
# Sat, 11 Feb 2023 07:47:38 GMT
ENV EGGDROP_COMMIT=2a6a36888f5aa2204d84a9e6282d35e5421c2c8a
# Sat, 11 Feb 2023 07:47:39 GMT
RUN apk --update add --no-cache bash openssl
# Sat, 11 Feb 2023 07:51:31 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 11 Feb 2023 07:51:31 GMT
ENV NICK=
# Sat, 11 Feb 2023 07:51:31 GMT
ENV SERVER=
# Sat, 11 Feb 2023 07:51:31 GMT
ENV LISTEN=3333
# Sat, 11 Feb 2023 07:51:31 GMT
ENV OWNER=
# Sat, 11 Feb 2023 07:51:31 GMT
ENV USERFILE=eggdrop.user
# Sat, 11 Feb 2023 07:51:32 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 11 Feb 2023 07:51:32 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 11 Feb 2023 07:51:32 GMT
EXPOSE 3333
# Sat, 11 Feb 2023 07:51:32 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Sat, 11 Feb 2023 07:51:32 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 11 Feb 2023 07:51:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 11 Feb 2023 07:51:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b4bba832da1fec1519d1be2d63ef0ffcc84d75b6db6df42c4c59d6bc7909f`  
		Last Modified: Sat, 11 Feb 2023 07:56:03 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc75a393c23b0e781af338ef981ff56ba6433c3207c9600ecfb5b0b5ef0b07b`  
		Last Modified: Sat, 11 Feb 2023 07:56:01 GMT  
		Size: 11.0 KB (10959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334aa6104162d045953c318a6a719bc3a96f1408bf6f8304b3daa2459e6a3f4b`  
		Last Modified: Sat, 11 Feb 2023 07:56:01 GMT  
		Size: 1.1 MB (1090108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ae2f8ea1a1ec72a7be9dfaf03a2b60e708c62bfc43330786b4b9611f2403ef`  
		Last Modified: Sat, 11 Feb 2023 07:56:03 GMT  
		Size: 10.7 MB (10687615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e861280f19c09b89f8a6cee053d730d9a6160de434bb76ff6a834729b1020c0`  
		Last Modified: Sat, 11 Feb 2023 07:56:01 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e6216bb55278efc253dfc07f10d507274448cd217b1fc1d093a50e98089c15`  
		Last Modified: Sat, 11 Feb 2023 07:56:01 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:e0fa47cfd9fa6dc31a394322cfd13f9987f5d25b1a5a0a712cf4fa2e3ddb9184
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14206582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d8ae3b78dc040b9b8f8cf2e7a0686df86b57d49f1aefa5d90915c0335ea9b5d`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:37:52 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 10 Feb 2023 21:37:53 GMT
RUN adduser -S eggdrop
# Fri, 10 Feb 2023 21:37:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 10 Feb 2023 21:37:54 GMT
ENV EGGDROP_SHA256=caafc1ad001e2e77793dca37998cb94d88efadb4ec9c3de44c1004b04f15aa6e
# Fri, 10 Feb 2023 21:37:54 GMT
ENV EGGDROP_COMMIT=2a6a36888f5aa2204d84a9e6282d35e5421c2c8a
# Fri, 10 Feb 2023 21:37:55 GMT
RUN apk --update add --no-cache bash openssl
# Fri, 10 Feb 2023 21:42:32 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 10 Feb 2023 21:42:32 GMT
ENV NICK=
# Fri, 10 Feb 2023 21:42:32 GMT
ENV SERVER=
# Fri, 10 Feb 2023 21:42:32 GMT
ENV LISTEN=3333
# Fri, 10 Feb 2023 21:42:32 GMT
ENV OWNER=
# Fri, 10 Feb 2023 21:42:32 GMT
ENV USERFILE=eggdrop.user
# Fri, 10 Feb 2023 21:42:32 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 10 Feb 2023 21:42:33 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 10 Feb 2023 21:42:33 GMT
EXPOSE 3333
# Fri, 10 Feb 2023 21:42:33 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Fri, 10 Feb 2023 21:42:33 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 10 Feb 2023 21:42:33 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 10 Feb 2023 21:42:33 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f307beb202bf7bcb9f58f8618b7432e52e14968b9385535f4e39797968d74f8b`  
		Last Modified: Fri, 10 Feb 2023 21:48:21 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a354c31f5821795ab52a25590b1f334e39b185b48944b37a40bf24f00adae7b`  
		Last Modified: Fri, 10 Feb 2023 21:48:19 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c85aa1c4a6fd356326cfbd33efa281fbe307459395fa44f8c93d2153dbabe`  
		Last Modified: Fri, 10 Feb 2023 21:48:20 GMT  
		Size: 1.0 MB (1032643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f546ee4bee6b79f21ef60660bef00537300c078242686b5c1d674b037c5710`  
		Last Modified: Fri, 10 Feb 2023 21:48:22 GMT  
		Size: 10.5 MB (10525426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c8e523cbc37eca1c7d4c4fa5fc103e59c9967de70527dfb74123834a4573aa`  
		Last Modified: Fri, 10 Feb 2023 21:48:19 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5047508085650a4453fb14e59e7833d27def38a4274ab51871b3ffd257d5c4`  
		Last Modified: Fri, 10 Feb 2023 21:48:19 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:26af7de37409a702a7bd1048793bcd79b6f4e09009b868fc8416b8f5b56dbf93
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14550585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7ba771920e448dac75c2718eefb8f3804c256a950370983d0267c774f31e5b4`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:10:49 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 10 Feb 2023 22:10:50 GMT
RUN adduser -S eggdrop
# Fri, 10 Feb 2023 22:10:51 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 10 Feb 2023 22:10:51 GMT
ENV EGGDROP_SHA256=caafc1ad001e2e77793dca37998cb94d88efadb4ec9c3de44c1004b04f15aa6e
# Fri, 10 Feb 2023 22:10:51 GMT
ENV EGGDROP_COMMIT=2a6a36888f5aa2204d84a9e6282d35e5421c2c8a
# Fri, 10 Feb 2023 22:10:52 GMT
RUN apk --update add --no-cache bash openssl
# Fri, 10 Feb 2023 22:14:41 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 10 Feb 2023 22:14:41 GMT
ENV NICK=
# Fri, 10 Feb 2023 22:14:41 GMT
ENV SERVER=
# Fri, 10 Feb 2023 22:14:41 GMT
ENV LISTEN=3333
# Fri, 10 Feb 2023 22:14:41 GMT
ENV OWNER=
# Fri, 10 Feb 2023 22:14:41 GMT
ENV USERFILE=eggdrop.user
# Fri, 10 Feb 2023 22:14:42 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 10 Feb 2023 22:14:42 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 10 Feb 2023 22:14:42 GMT
EXPOSE 3333
# Fri, 10 Feb 2023 22:14:42 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Fri, 10 Feb 2023 22:14:42 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 10 Feb 2023 22:14:42 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 10 Feb 2023 22:14:42 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8186b969b70bfd3a8f8529034203efaf95ad8eddf3c33fb41cf503890b1700b`  
		Last Modified: Fri, 10 Feb 2023 22:19:00 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212afe5219f2149a8e95b00c1346982e164235c46e289d221ac1897ca9048c2f`  
		Last Modified: Fri, 10 Feb 2023 22:18:58 GMT  
		Size: 10.8 KB (10769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166b6dcf0dd4056b6515bde1969fd9a9008e4ada399c4be2c520075ebedf32c1`  
		Last Modified: Fri, 10 Feb 2023 22:18:59 GMT  
		Size: 1.1 MB (1087885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574ab5da52d2e1338b4d9359da1ce06f3ac8e7c13ca6642062bd8c97bb50784a`  
		Last Modified: Fri, 10 Feb 2023 22:19:00 GMT  
		Size: 10.7 MB (10726155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0658130289555357b4bcc32867d0e841e43ac3fd260ec6a79cea1100c2137330`  
		Last Modified: Fri, 10 Feb 2023 22:18:59 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3515ad107ce1fa3f7bc67db346f13973d805d0f9d98ffbe4de99c20385698aa7`  
		Last Modified: Fri, 10 Feb 2023 22:18:58 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
