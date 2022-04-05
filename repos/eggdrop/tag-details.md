<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.2`](#eggdrop192)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:faa227d56547d3820922135762c6ab1f39d5b25f6566848bf9a8bd7439571e7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:3b8f3d6d8d54caf3481cfa1460600229fc8c6da8e910fdbb99e39a74e56d020c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8284963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7e75710541da8025bad1f0029c3ca1af5388a757b7d20e89aca2a003e65400`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:16:32 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 11:16:33 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 11:16:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 11:16:35 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 11:17:25 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 11:17:26 GMT
ENV NICK=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV SERVER=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 11:17:26 GMT
ENV OWNER=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 11:17:26 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 11:17:26 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 11:17:26 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 11:17:26 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 11:17:26 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 11:17:27 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 11:17:27 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af7270901fcd1dae05f35973cd7825724dbc1bd998e39f5d71450e974a3153`  
		Last Modified: Tue, 05 Apr 2022 11:17:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa006e8c5e3fd9de6d58e77396feb8a3bc4a41181f023dfaaa0ff5ea2394ae7`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 10.7 KB (10703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356ac0c96e4675ed17f71ab61eb3b7302184d902b4c8b03940a9455937005aa`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 2.7 MB (2726450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa54252a0927aac784047d4bb711cdb2300cf0ab2cb717b6a6c39d5f09d16274`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 2.7 MB (2724699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefa2626779fae87079a5346e23ce3c837754cf74b4480391cc1fab89653b435`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c0dcfa91e1ea98c3a706cdb4c1caa0529339cc39fea214f12d278212eda12`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:5f612a73564453d842b4d792dc9ae6e4242412b5b7a032b475c5be472d28e6d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7975642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf5abfb1dcefa42801e88040dbbcf28f1a958831415925b1b8f6be8fffc8808`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:42:42 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 03:42:43 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 03:42:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 03:42:49 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 03:45:10 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 03:45:10 GMT
ENV NICK=
# Tue, 05 Apr 2022 03:45:11 GMT
ENV SERVER=
# Tue, 05 Apr 2022 03:45:11 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 03:45:12 GMT
ENV OWNER=
# Tue, 05 Apr 2022 03:45:12 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 03:45:12 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 03:45:13 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 03:45:13 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 03:45:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 03:45:14 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 03:45:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 03:45:15 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216d0875ece6437b7759f658b19a743c65d8a0209dd6959b89006f06a7d4632d`  
		Last Modified: Tue, 05 Apr 2022 03:46:25 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb2483aeba1bc6bf4edfd57deb0a196f319c5338bf1032faa780a5f7d392477`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 10.4 KB (10403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883dd4bb4066fb7e7baa70d4271a40c7d91977982d50cc6b30892462da59f8b`  
		Last Modified: Tue, 05 Apr 2022 03:46:26 GMT  
		Size: 2.7 MB (2653002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c32b092000a7f5deeebdd19f48bf387342a0106dd81e475ba6110f073171679`  
		Last Modified: Tue, 05 Apr 2022 03:46:26 GMT  
		Size: 2.7 MB (2683288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45089181a50f12a8dcd62efc9ad43f63605aece6c118eddafefa51dfb361fc4`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43385cdd604f9bac361f23a6a138a6e0e979410600f0c9a4d4fc9f564b16e1a`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:a63be8915ecee00600434fbae83c83b8826ccf9163773af37a6529e5a9b4e5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8206988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef7a72401b0431e568de59619be3e4194fd339d58d0312252354c864238658e`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:08:50 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 04:08:51 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 04:08:53 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 04:08:55 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 04:10:00 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 04:10:01 GMT
ENV NICK=
# Tue, 05 Apr 2022 04:10:02 GMT
ENV SERVER=
# Tue, 05 Apr 2022 04:10:03 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 04:10:04 GMT
ENV OWNER=
# Tue, 05 Apr 2022 04:10:05 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 04:10:06 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 04:10:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 04:10:08 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 04:10:10 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 04:10:11 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 04:10:11 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 04:10:12 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad29698dd37ab923ffb59ccb8a25101399ae72afc52716f7abef24b92f50f6f8`  
		Last Modified: Tue, 05 Apr 2022 04:10:46 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8e549fca9947f4bb9b0c7445e2dec0e1372dcfcf71a2845b36869e8b5213a1`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 10.5 KB (10481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019a83cb70204edfbb029b1bf19a37c13268c06f97b77a3e4a687d3ebdd9ba3f`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 2.8 MB (2752068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1050eba79944e68ab2dec5b7978af9ef6ee179979ad364e1c6c8a578bc5ba17`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 2.7 MB (2719773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec4e36daf9711164139c38e07f155b97f78ed76f76927146f1a8d483a1979e8`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035e6d3d5202a896ef25b0b1b67b32e046ec78a3f72d91637944160d57abff50`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.2`

```console
$ docker pull eggdrop@sha256:faa227d56547d3820922135762c6ab1f39d5b25f6566848bf9a8bd7439571e7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9.2` - linux; amd64

```console
$ docker pull eggdrop@sha256:3b8f3d6d8d54caf3481cfa1460600229fc8c6da8e910fdbb99e39a74e56d020c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8284963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7e75710541da8025bad1f0029c3ca1af5388a757b7d20e89aca2a003e65400`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:16:32 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 11:16:33 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 11:16:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 11:16:35 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 11:17:25 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 11:17:26 GMT
ENV NICK=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV SERVER=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 11:17:26 GMT
ENV OWNER=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 11:17:26 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 11:17:26 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 11:17:26 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 11:17:26 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 11:17:26 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 11:17:27 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 11:17:27 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af7270901fcd1dae05f35973cd7825724dbc1bd998e39f5d71450e974a3153`  
		Last Modified: Tue, 05 Apr 2022 11:17:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa006e8c5e3fd9de6d58e77396feb8a3bc4a41181f023dfaaa0ff5ea2394ae7`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 10.7 KB (10703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356ac0c96e4675ed17f71ab61eb3b7302184d902b4c8b03940a9455937005aa`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 2.7 MB (2726450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa54252a0927aac784047d4bb711cdb2300cf0ab2cb717b6a6c39d5f09d16274`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 2.7 MB (2724699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefa2626779fae87079a5346e23ce3c837754cf74b4480391cc1fab89653b435`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c0dcfa91e1ea98c3a706cdb4c1caa0529339cc39fea214f12d278212eda12`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.2` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:5f612a73564453d842b4d792dc9ae6e4242412b5b7a032b475c5be472d28e6d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7975642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf5abfb1dcefa42801e88040dbbcf28f1a958831415925b1b8f6be8fffc8808`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:42:42 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 03:42:43 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 03:42:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 03:42:49 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 03:45:10 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 03:45:10 GMT
ENV NICK=
# Tue, 05 Apr 2022 03:45:11 GMT
ENV SERVER=
# Tue, 05 Apr 2022 03:45:11 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 03:45:12 GMT
ENV OWNER=
# Tue, 05 Apr 2022 03:45:12 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 03:45:12 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 03:45:13 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 03:45:13 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 03:45:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 03:45:14 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 03:45:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 03:45:15 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216d0875ece6437b7759f658b19a743c65d8a0209dd6959b89006f06a7d4632d`  
		Last Modified: Tue, 05 Apr 2022 03:46:25 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb2483aeba1bc6bf4edfd57deb0a196f319c5338bf1032faa780a5f7d392477`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 10.4 KB (10403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883dd4bb4066fb7e7baa70d4271a40c7d91977982d50cc6b30892462da59f8b`  
		Last Modified: Tue, 05 Apr 2022 03:46:26 GMT  
		Size: 2.7 MB (2653002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c32b092000a7f5deeebdd19f48bf387342a0106dd81e475ba6110f073171679`  
		Last Modified: Tue, 05 Apr 2022 03:46:26 GMT  
		Size: 2.7 MB (2683288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45089181a50f12a8dcd62efc9ad43f63605aece6c118eddafefa51dfb361fc4`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43385cdd604f9bac361f23a6a138a6e0e979410600f0c9a4d4fc9f564b16e1a`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.2` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:a63be8915ecee00600434fbae83c83b8826ccf9163773af37a6529e5a9b4e5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8206988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef7a72401b0431e568de59619be3e4194fd339d58d0312252354c864238658e`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:08:50 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 04:08:51 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 04:08:53 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 04:08:55 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 04:10:00 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 04:10:01 GMT
ENV NICK=
# Tue, 05 Apr 2022 04:10:02 GMT
ENV SERVER=
# Tue, 05 Apr 2022 04:10:03 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 04:10:04 GMT
ENV OWNER=
# Tue, 05 Apr 2022 04:10:05 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 04:10:06 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 04:10:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 04:10:08 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 04:10:10 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 04:10:11 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 04:10:11 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 04:10:12 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad29698dd37ab923ffb59ccb8a25101399ae72afc52716f7abef24b92f50f6f8`  
		Last Modified: Tue, 05 Apr 2022 04:10:46 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8e549fca9947f4bb9b0c7445e2dec0e1372dcfcf71a2845b36869e8b5213a1`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 10.5 KB (10481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019a83cb70204edfbb029b1bf19a37c13268c06f97b77a3e4a687d3ebdd9ba3f`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 2.8 MB (2752068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1050eba79944e68ab2dec5b7978af9ef6ee179979ad364e1c6c8a578bc5ba17`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 2.7 MB (2719773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec4e36daf9711164139c38e07f155b97f78ed76f76927146f1a8d483a1979e8`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035e6d3d5202a896ef25b0b1b67b32e046ec78a3f72d91637944160d57abff50`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:29207d7afa95f48fb0ffc6cd2e2adcdf3f1f700477a2076d9c91ecb3016a6558
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:0ca3da0a17bdb08cf0b4a568e67f4300a992968802fd235e80244289061c7bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39770884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5df690ac22fa1cc6aa8382293476ca5a98fd60ae3d66783e8ddd140aef59800`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:12:25 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 11:12:25 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 11:12:26 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 11:12:26 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Tue, 05 Apr 2022 11:12:26 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Tue, 05 Apr 2022 11:12:27 GMT
RUN apk --update add --no-cache bash openssl
# Tue, 05 Apr 2022 11:16:15 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 11:16:15 GMT
ENV NICK=
# Tue, 05 Apr 2022 11:16:15 GMT
ENV SERVER=
# Tue, 05 Apr 2022 11:16:15 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 11:16:15 GMT
ENV OWNER=
# Tue, 05 Apr 2022 11:16:15 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 11:16:16 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 11:16:16 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 11:16:16 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 11:16:16 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 11:16:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 11:16:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 11:16:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afb7ebc822c4005d25f15d49dada11e4a41876f643351d04feea9b2b22840cc`  
		Last Modified: Tue, 05 Apr 2022 11:17:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e7bd2972241b11e355dd2e732c2f4dbcbe0a9624d7b8c43e68e1b891810d4a`  
		Last Modified: Tue, 05 Apr 2022 11:17:38 GMT  
		Size: 10.9 KB (10946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fd22df8199a256e85c584df095acfc186d61699ad6b8e96604ea1e648ecc01`  
		Last Modified: Tue, 05 Apr 2022 11:17:39 GMT  
		Size: 1.1 MB (1089643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a191850056d4a640017fa13982a3c9dcb30e121e493cb1cf7afd10369ee8fea3`  
		Last Modified: Tue, 05 Apr 2022 11:17:44 GMT  
		Size: 35.9 MB (35851891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbdce544ebf06c5f556efde720928e8ed4aa86d0c56136b27c5f0e155bc2420`  
		Last Modified: Tue, 05 Apr 2022 11:17:38 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f2a8e43de6502d7ca7f10e7452d93fdfbef0b6800803256dfb73aaf711a0bf`  
		Last Modified: Tue, 05 Apr 2022 11:17:38 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:d44ee11b7644f8abc0a45dd6a217bf889ba0609c4d821752f914b82f36f906f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39165975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3b0ecf2e6aae1404fb2c832457e6b21f9104ad254f831964b14b688212fb09`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:31:44 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 03:31:46 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 03:31:48 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 03:31:49 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Tue, 05 Apr 2022 03:31:49 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Tue, 05 Apr 2022 03:31:52 GMT
RUN apk --update add --no-cache bash openssl
# Tue, 05 Apr 2022 03:42:15 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 03:42:16 GMT
ENV NICK=
# Tue, 05 Apr 2022 03:42:16 GMT
ENV SERVER=
# Tue, 05 Apr 2022 03:42:17 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 03:42:17 GMT
ENV OWNER=
# Tue, 05 Apr 2022 03:42:18 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 03:42:18 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 03:42:19 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 03:42:19 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 03:42:20 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 03:42:20 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 03:42:21 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 03:42:21 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f46acd206d1b9854dd7a69f3dd94d51ffb03228b347337d6755524e938f848d`  
		Last Modified: Tue, 05 Apr 2022 03:45:57 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ab9123d31326e4f773e35061abb57883ec6b6221e6df8719354fc8598c9123`  
		Last Modified: Tue, 05 Apr 2022 03:45:55 GMT  
		Size: 10.6 KB (10643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f62deb3100b6e70cd59c7464cb4b29e2b0838161967661ab0f746b51836a177`  
		Last Modified: Tue, 05 Apr 2022 03:45:56 GMT  
		Size: 1.0 MB (1032380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc277f2652bea54f29023ad9ac96a2bb389a9ccf2e329165f706ec56ea3f56f9`  
		Last Modified: Tue, 05 Apr 2022 03:46:16 GMT  
		Size: 35.5 MB (35497123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c017a0ffbca5f124cc57390d8252246ef4d6816998bb3a6a2803283b7c410e4`  
		Last Modified: Tue, 05 Apr 2022 03:45:55 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbe5ead144b0f664d6067b076f6aafeee3934feae5435527f1094d3c70d7dee`  
		Last Modified: Tue, 05 Apr 2022 03:45:55 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:58f83502c20b55f1671395b5223199de3f924fb00bac184289616356097c3538
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39840336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:517417f6c33ea4e8eda7d28e039ac194c20d366292a9fcaacb84af1a9c259985`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:03:36 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 04:03:37 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 04:03:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 04:03:39 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Tue, 05 Apr 2022 04:03:40 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Tue, 05 Apr 2022 04:03:41 GMT
RUN apk --update add --no-cache bash openssl
# Tue, 05 Apr 2022 04:08:22 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 04:08:22 GMT
ENV NICK=
# Tue, 05 Apr 2022 04:08:23 GMT
ENV SERVER=
# Tue, 05 Apr 2022 04:08:24 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 04:08:25 GMT
ENV OWNER=
# Tue, 05 Apr 2022 04:08:26 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 04:08:27 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 04:08:28 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 04:08:29 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 04:08:31 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 04:08:32 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 04:08:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 04:08:33 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687fbd14cec7fbb8ee2d3dfd1bedd832165c780a579635649359ea5d966007c3`  
		Last Modified: Tue, 05 Apr 2022 04:10:33 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778e0ebd563495b9fbda0eb57ed55b539e2a45c085cbb1dc1866b09b01007cb8`  
		Last Modified: Tue, 05 Apr 2022 04:10:31 GMT  
		Size: 10.7 KB (10674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dd87a81b82b563a55309efc83e5bd1449b7594eca26057853510451078447f`  
		Last Modified: Tue, 05 Apr 2022 04:10:31 GMT  
		Size: 1.1 MB (1087188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf6a2b0c72c2b5112ebe5cf3034eb8be33586e208322d0534280410057a0766`  
		Last Modified: Tue, 05 Apr 2022 04:10:36 GMT  
		Size: 36.0 MB (36022170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b64c592a79e2e4db70bb2315b6a98f3746dffe89a10745de53586994195e89`  
		Last Modified: Tue, 05 Apr 2022 04:10:31 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b44e16d37a27f754c949073353a7972c76ba0ef406b0b24db57f8fca427df18`  
		Last Modified: Tue, 05 Apr 2022 04:10:31 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:faa227d56547d3820922135762c6ab1f39d5b25f6566848bf9a8bd7439571e7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:3b8f3d6d8d54caf3481cfa1460600229fc8c6da8e910fdbb99e39a74e56d020c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8284963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7e75710541da8025bad1f0029c3ca1af5388a757b7d20e89aca2a003e65400`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:16:32 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 11:16:33 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 11:16:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 11:16:35 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 11:17:25 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 11:17:26 GMT
ENV NICK=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV SERVER=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 11:17:26 GMT
ENV OWNER=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 11:17:26 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 11:17:26 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 11:17:26 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 11:17:26 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 11:17:26 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 11:17:27 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 11:17:27 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af7270901fcd1dae05f35973cd7825724dbc1bd998e39f5d71450e974a3153`  
		Last Modified: Tue, 05 Apr 2022 11:17:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa006e8c5e3fd9de6d58e77396feb8a3bc4a41181f023dfaaa0ff5ea2394ae7`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 10.7 KB (10703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356ac0c96e4675ed17f71ab61eb3b7302184d902b4c8b03940a9455937005aa`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 2.7 MB (2726450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa54252a0927aac784047d4bb711cdb2300cf0ab2cb717b6a6c39d5f09d16274`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 2.7 MB (2724699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefa2626779fae87079a5346e23ce3c837754cf74b4480391cc1fab89653b435`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c0dcfa91e1ea98c3a706cdb4c1caa0529339cc39fea214f12d278212eda12`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:5f612a73564453d842b4d792dc9ae6e4242412b5b7a032b475c5be472d28e6d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7975642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf5abfb1dcefa42801e88040dbbcf28f1a958831415925b1b8f6be8fffc8808`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:42:42 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 03:42:43 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 03:42:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 03:42:49 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 03:45:10 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 03:45:10 GMT
ENV NICK=
# Tue, 05 Apr 2022 03:45:11 GMT
ENV SERVER=
# Tue, 05 Apr 2022 03:45:11 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 03:45:12 GMT
ENV OWNER=
# Tue, 05 Apr 2022 03:45:12 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 03:45:12 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 03:45:13 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 03:45:13 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 03:45:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 03:45:14 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 03:45:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 03:45:15 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216d0875ece6437b7759f658b19a743c65d8a0209dd6959b89006f06a7d4632d`  
		Last Modified: Tue, 05 Apr 2022 03:46:25 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb2483aeba1bc6bf4edfd57deb0a196f319c5338bf1032faa780a5f7d392477`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 10.4 KB (10403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883dd4bb4066fb7e7baa70d4271a40c7d91977982d50cc6b30892462da59f8b`  
		Last Modified: Tue, 05 Apr 2022 03:46:26 GMT  
		Size: 2.7 MB (2653002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c32b092000a7f5deeebdd19f48bf387342a0106dd81e475ba6110f073171679`  
		Last Modified: Tue, 05 Apr 2022 03:46:26 GMT  
		Size: 2.7 MB (2683288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45089181a50f12a8dcd62efc9ad43f63605aece6c118eddafefa51dfb361fc4`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43385cdd604f9bac361f23a6a138a6e0e979410600f0c9a4d4fc9f564b16e1a`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:a63be8915ecee00600434fbae83c83b8826ccf9163773af37a6529e5a9b4e5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8206988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef7a72401b0431e568de59619be3e4194fd339d58d0312252354c864238658e`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:08:50 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 04:08:51 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 04:08:53 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 04:08:55 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 04:10:00 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 04:10:01 GMT
ENV NICK=
# Tue, 05 Apr 2022 04:10:02 GMT
ENV SERVER=
# Tue, 05 Apr 2022 04:10:03 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 04:10:04 GMT
ENV OWNER=
# Tue, 05 Apr 2022 04:10:05 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 04:10:06 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 04:10:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 04:10:08 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 04:10:10 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 04:10:11 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 04:10:11 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 04:10:12 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad29698dd37ab923ffb59ccb8a25101399ae72afc52716f7abef24b92f50f6f8`  
		Last Modified: Tue, 05 Apr 2022 04:10:46 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8e549fca9947f4bb9b0c7445e2dec0e1372dcfcf71a2845b36869e8b5213a1`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 10.5 KB (10481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019a83cb70204edfbb029b1bf19a37c13268c06f97b77a3e4a687d3ebdd9ba3f`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 2.8 MB (2752068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1050eba79944e68ab2dec5b7978af9ef6ee179979ad364e1c6c8a578bc5ba17`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 2.7 MB (2719773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec4e36daf9711164139c38e07f155b97f78ed76f76927146f1a8d483a1979e8`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035e6d3d5202a896ef25b0b1b67b32e046ec78a3f72d91637944160d57abff50`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:faa227d56547d3820922135762c6ab1f39d5b25f6566848bf9a8bd7439571e7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:3b8f3d6d8d54caf3481cfa1460600229fc8c6da8e910fdbb99e39a74e56d020c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8284963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7e75710541da8025bad1f0029c3ca1af5388a757b7d20e89aca2a003e65400`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:16:32 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 11:16:33 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 11:16:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 11:16:35 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 11:17:25 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 11:17:26 GMT
ENV NICK=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV SERVER=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 11:17:26 GMT
ENV OWNER=
# Tue, 05 Apr 2022 11:17:26 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 11:17:26 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 11:17:26 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 11:17:26 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 11:17:26 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 11:17:26 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 11:17:27 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 11:17:27 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af7270901fcd1dae05f35973cd7825724dbc1bd998e39f5d71450e974a3153`  
		Last Modified: Tue, 05 Apr 2022 11:17:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa006e8c5e3fd9de6d58e77396feb8a3bc4a41181f023dfaaa0ff5ea2394ae7`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 10.7 KB (10703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2356ac0c96e4675ed17f71ab61eb3b7302184d902b4c8b03940a9455937005aa`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 2.7 MB (2726450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa54252a0927aac784047d4bb711cdb2300cf0ab2cb717b6a6c39d5f09d16274`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 2.7 MB (2724699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefa2626779fae87079a5346e23ce3c837754cf74b4480391cc1fab89653b435`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c0dcfa91e1ea98c3a706cdb4c1caa0529339cc39fea214f12d278212eda12`  
		Last Modified: Tue, 05 Apr 2022 11:17:51 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:5f612a73564453d842b4d792dc9ae6e4242412b5b7a032b475c5be472d28e6d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7975642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf5abfb1dcefa42801e88040dbbcf28f1a958831415925b1b8f6be8fffc8808`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:42:42 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 03:42:43 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 03:42:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 03:42:49 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 03:45:10 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 03:45:10 GMT
ENV NICK=
# Tue, 05 Apr 2022 03:45:11 GMT
ENV SERVER=
# Tue, 05 Apr 2022 03:45:11 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 03:45:12 GMT
ENV OWNER=
# Tue, 05 Apr 2022 03:45:12 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 03:45:12 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 03:45:13 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 03:45:13 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 03:45:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 03:45:14 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 03:45:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 03:45:15 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216d0875ece6437b7759f658b19a743c65d8a0209dd6959b89006f06a7d4632d`  
		Last Modified: Tue, 05 Apr 2022 03:46:25 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb2483aeba1bc6bf4edfd57deb0a196f319c5338bf1032faa780a5f7d392477`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 10.4 KB (10403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883dd4bb4066fb7e7baa70d4271a40c7d91977982d50cc6b30892462da59f8b`  
		Last Modified: Tue, 05 Apr 2022 03:46:26 GMT  
		Size: 2.7 MB (2653002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c32b092000a7f5deeebdd19f48bf387342a0106dd81e475ba6110f073171679`  
		Last Modified: Tue, 05 Apr 2022 03:46:26 GMT  
		Size: 2.7 MB (2683288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45089181a50f12a8dcd62efc9ad43f63605aece6c118eddafefa51dfb361fc4`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43385cdd604f9bac361f23a6a138a6e0e979410600f0c9a4d4fc9f564b16e1a`  
		Last Modified: Tue, 05 Apr 2022 03:46:24 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:a63be8915ecee00600434fbae83c83b8826ccf9163773af37a6529e5a9b4e5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8206988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef7a72401b0431e568de59619be3e4194fd339d58d0312252354c864238658e`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:08:50 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 05 Apr 2022 04:08:51 GMT
RUN adduser -S eggdrop
# Tue, 05 Apr 2022 04:08:53 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 05 Apr 2022 04:08:55 GMT
RUN apk add --no-cache tcl bash openssl
# Tue, 05 Apr 2022 04:10:00 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 05 Apr 2022 04:10:01 GMT
ENV NICK=
# Tue, 05 Apr 2022 04:10:02 GMT
ENV SERVER=
# Tue, 05 Apr 2022 04:10:03 GMT
ENV LISTEN=3333
# Tue, 05 Apr 2022 04:10:04 GMT
ENV OWNER=
# Tue, 05 Apr 2022 04:10:05 GMT
ENV USERFILE=eggdrop.user
# Tue, 05 Apr 2022 04:10:06 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 05 Apr 2022 04:10:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 05 Apr 2022 04:10:08 GMT
EXPOSE 3333
# Tue, 05 Apr 2022 04:10:10 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 05 Apr 2022 04:10:11 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 05 Apr 2022 04:10:11 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 05 Apr 2022 04:10:12 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad29698dd37ab923ffb59ccb8a25101399ae72afc52716f7abef24b92f50f6f8`  
		Last Modified: Tue, 05 Apr 2022 04:10:46 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8e549fca9947f4bb9b0c7445e2dec0e1372dcfcf71a2845b36869e8b5213a1`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 10.5 KB (10481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019a83cb70204edfbb029b1bf19a37c13268c06f97b77a3e4a687d3ebdd9ba3f`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 2.8 MB (2752068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1050eba79944e68ab2dec5b7978af9ef6ee179979ad364e1c6c8a578bc5ba17`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 2.7 MB (2719773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec4e36daf9711164139c38e07f155b97f78ed76f76927146f1a8d483a1979e8`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035e6d3d5202a896ef25b0b1b67b32e046ec78a3f72d91637944160d57abff50`  
		Last Modified: Tue, 05 Apr 2022 04:10:44 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
