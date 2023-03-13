## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:12ea1bd2bfd37a770c3a514bad1f1d19386134b26b1071f1b2fdc411578dc903
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:7d503e0bbbcf926621597e8442d5b75273ed5f51cbaebf5ca4c32e1cbca62d6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11707730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94885e42bceb6f392a87abdba804b2649c33d961d93aaa1cfd4ae23b75cdacdf`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:51:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 11 Feb 2023 07:51:46 GMT
RUN adduser -S eggdrop
# Sat, 11 Feb 2023 07:51:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 11 Feb 2023 07:51:48 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 11 Feb 2023 07:55:46 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 11 Feb 2023 07:55:46 GMT
ENV NICK=
# Sat, 11 Feb 2023 07:55:46 GMT
ENV SERVER=
# Sat, 11 Feb 2023 07:55:47 GMT
ENV LISTEN=3333
# Sat, 11 Feb 2023 07:55:47 GMT
ENV OWNER=
# Sat, 11 Feb 2023 07:55:47 GMT
ENV USERFILE=eggdrop.user
# Sat, 11 Feb 2023 07:55:47 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 11 Feb 2023 07:55:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 11 Feb 2023 07:55:47 GMT
EXPOSE 3333
# Sat, 11 Feb 2023 07:55:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 11 Feb 2023 07:55:47 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 11 Feb 2023 07:55:47 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 11 Feb 2023 07:55:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5929d6c17ae9e3c1785e747f2e1c9a4043d1271b0b4fa46fd3b5d69e688807c3`  
		Last Modified: Sat, 11 Feb 2023 07:56:10 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45534f8d250972e326ebb489c727bd241fe3ff4b1127eb39d1d672b0168cca9e`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 10.9 KB (10932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c10f44dd07312e4c61cf11012690bfbb08c68a17c2cbd5e4c5bec99e2dcecf`  
		Last Modified: Sat, 11 Feb 2023 07:56:09 GMT  
		Size: 2.8 MB (2757983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da126ee1240a822d73b85fe7646d08199ddab22146b346b6082d64822089bbfa`  
		Last Modified: Sat, 11 Feb 2023 07:56:09 GMT  
		Size: 6.1 MB (6127248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97460e3eba8e8c667065808ae8282c0b7ddf147ddae13b3a5553a431bcccdd0`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f385e4dbc86989aa993e14712f5523b1dd3458d9c4b311d202765f34873e60`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:add1154fcd484e80e959a680b538c3bfd2a25aedc5e2db342f32572170880ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11352013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da83a66d4ecc8fc4b5598adbac4cd7c21311a640733c0db906a4b0b9a6a8dba`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 17:12:15 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 13 Mar 2023 17:12:16 GMT
RUN adduser -S eggdrop
# Mon, 13 Mar 2023 17:12:17 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 13 Mar 2023 17:12:19 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 13 Mar 2023 17:16:35 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 17:16:35 GMT
ENV NICK=
# Mon, 13 Mar 2023 17:16:35 GMT
ENV SERVER=
# Mon, 13 Mar 2023 17:16:35 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 17:16:36 GMT
ENV OWNER=
# Mon, 13 Mar 2023 17:16:36 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 17:16:36 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 17:16:36 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 17:16:36 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 17:16:36 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 17:16:36 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 17:16:36 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 17:16:36 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec2417a5f95cb8476bdb0bd490a3653224f7fbdf8ed2d8ad59f0de673e0d67`  
		Last Modified: Mon, 13 Mar 2023 17:17:05 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f559d903a28746e7b2cf18297c1dbd3ed8df78227b31a55764027bb8c88190`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 10.6 KB (10638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f4bd0129aa84d8df20f9b5ed48a4a123ec3cc83121d834bc9e5e55e32a2373`  
		Last Modified: Mon, 13 Mar 2023 17:17:04 GMT  
		Size: 2.7 MB (2679912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca42b7876bf72171c45ac71c6d89f12218cc82ee2bea7227ea98efef4b97d22`  
		Last Modified: Mon, 13 Mar 2023 17:17:05 GMT  
		Size: 6.0 MB (6040868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e353d64f03127a8631c30ac73e868b707101a590d5b35332915ce50036835c`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9ed6c536151b03b35d7e2c5575691fc2f72693d3d8ad65af13ab3414df0490`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:1c7967dde971d677a4171a266645bebd6cc600eef70813b3accd66d4d2b45ae2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11668449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a4af97b3fefa9ed49c50147740fa45b6aefa32e3af0099bdef5807c5c6ea782`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:57 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 10 Feb 2023 22:14:58 GMT
RUN adduser -S eggdrop
# Fri, 10 Feb 2023 22:14:59 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 10 Feb 2023 22:15:00 GMT
RUN apk add --no-cache tcl bash openssl
# Fri, 10 Feb 2023 22:18:43 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 10 Feb 2023 22:18:43 GMT
ENV NICK=
# Fri, 10 Feb 2023 22:18:43 GMT
ENV SERVER=
# Fri, 10 Feb 2023 22:18:43 GMT
ENV LISTEN=3333
# Fri, 10 Feb 2023 22:18:44 GMT
ENV OWNER=
# Fri, 10 Feb 2023 22:18:44 GMT
ENV USERFILE=eggdrop.user
# Fri, 10 Feb 2023 22:18:44 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 10 Feb 2023 22:18:44 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 10 Feb 2023 22:18:44 GMT
EXPOSE 3333
# Fri, 10 Feb 2023 22:18:44 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Fri, 10 Feb 2023 22:18:44 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 10 Feb 2023 22:18:44 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 10 Feb 2023 22:18:44 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb182a5cc1394eccbeeef59c5ad5d259ed5ddd4cdd2a1d4c5ad107256b7a2ee`  
		Last Modified: Fri, 10 Feb 2023 22:19:08 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59923206b30ea4054c1bb753aa8a5404a199d12f865dc365b1f8eb66fdb817b`  
		Last Modified: Fri, 10 Feb 2023 22:19:06 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd68e4187ad121351dbe2536603e4802110332e9e21ecccff44b92d2ea68b5`  
		Last Modified: Fri, 10 Feb 2023 22:19:07 GMT  
		Size: 2.8 MB (2776467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7285c61bf7d00d3cc40563b07cc910cfc6f1cbf6c20e0aa7b1b56e3ed8c069d`  
		Last Modified: Fri, 10 Feb 2023 22:19:07 GMT  
		Size: 6.2 MB (6167927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14d023f19ac2bdabff1a6f56426d0cd6782fe4048edf76831b7c32e64f915b2`  
		Last Modified: Fri, 10 Feb 2023 22:19:06 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b282c5ded3cb4dd851d61d8a68894034bc8279f449025b2ad2c0b4a6e9361cc6`  
		Last Modified: Fri, 10 Feb 2023 22:19:06 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
