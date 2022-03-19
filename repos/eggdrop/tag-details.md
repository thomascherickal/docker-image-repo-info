<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.2`](#eggdrop192)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:1fa1f45990945b00fdf398a825c1868736b37dd0605affcd075a51a1f76b1ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:a9b09dad37a7d351adf38d5a3235c12af1ed3564b73aac2ba748d58e345376b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8282046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9dd1bbf14a48744b1dec02b68a901079951585fe36d1e87218895d262d98516`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:05:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 19 Mar 2022 03:05:37 GMT
RUN adduser -S eggdrop
# Sat, 19 Mar 2022 03:05:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 03:05:39 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 19 Mar 2022 03:07:15 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 19 Mar 2022 03:07:15 GMT
ENV NICK=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV SERVER=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV LISTEN=3333
# Sat, 19 Mar 2022 03:07:15 GMT
ENV OWNER=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV USERFILE=eggdrop.user
# Sat, 19 Mar 2022 03:07:15 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 19 Mar 2022 03:07:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 19 Mar 2022 03:07:15 GMT
EXPOSE 3333
# Sat, 19 Mar 2022 03:07:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 19 Mar 2022 03:07:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 19 Mar 2022 03:07:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 19 Mar 2022 03:07:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cef478d9d2e17c2069b3b787f432f66639b715bbf9fc9be426ae6aa3ef59c2f`  
		Last Modified: Sat, 19 Mar 2022 03:07:41 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389bcdf8f16100f8d9c2358a3cf00ce0b5cd27b98ddf4951213e6b6349c73c6b`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 10.7 KB (10701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f092587418f14c475253126c75b2c2f98611f67d66a9df545bdfcd79f63ecb54`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 2.7 MB (2725676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a220e2a1485d9064ab75a27e36c756f0dc76c045749f01bf95fbf2d4b13398`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 2.7 MB (2724694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdb7391b21cc18aa21e66bdbaf6dfa1f09c6008cf67bc5e6967caff6a6fb038`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6526ffbb05a9b20439dce8e5c1749c8e6b36f1de10ae3c4570ea9c18821e088`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:122bb0227f48ef8fe35ba5812cb8958afb24465ccfd5c7ac68be28f5a63b204d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7978193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a651c413330366ccced3e0f0ef84e38f1bbfa847251f4d46b94f11379d9dad`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:15:44 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Mar 2022 15:15:45 GMT
RUN adduser -S eggdrop
# Thu, 17 Mar 2022 15:15:47 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Mar 2022 15:15:50 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Mar 2022 15:18:23 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Mar 2022 15:18:24 GMT
ENV NICK=
# Thu, 17 Mar 2022 15:18:24 GMT
ENV SERVER=
# Thu, 17 Mar 2022 15:18:24 GMT
ENV LISTEN=3333
# Thu, 17 Mar 2022 15:18:25 GMT
ENV OWNER=
# Thu, 17 Mar 2022 15:18:25 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Mar 2022 15:18:26 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Mar 2022 15:18:26 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Mar 2022 15:18:26 GMT
EXPOSE 3333
# Thu, 17 Mar 2022 15:18:27 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 17 Mar 2022 15:18:27 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Mar 2022 15:18:28 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Mar 2022 15:18:28 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1e510cf840340b9c34cfa14cc3fc7a832572443f28af0d2c63cf30dec078`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cb7fa74ab74933c3d0f5a43b2b2e0f5cb4332ad9e0f3d558b3bc296e438dad`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 10.4 KB (10402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce325b134d392e303241c318e8f3927c9fff71180df7ab82013df55879374047`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 2.7 MB (2652778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12377e78aa28c481d5f31d50a704199e7a8ece0d814e51692670d1dfcdf210`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 2.7 MB (2683288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0311035445d15202ed8f1d5d853071ea99fcd4919d47c93ffe8b3dd72cf901`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df94df2aefc0ab73ed8cdc9d8e440c91a76a178bc7a7e93c2564e770d5a22bb`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c238c47c3943e2433b9b4b521d1216015d5382efcfd6b2f205b2b3811e578b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8205326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3360c1069756788284a40b6b4d98d5c5524e0831045b8c9f7fc6c4390ca8c7d`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:45:12 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 18 Mar 2022 14:45:13 GMT
RUN adduser -S eggdrop
# Fri, 18 Mar 2022 14:45:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 18 Mar 2022 14:45:16 GMT
RUN apk add --no-cache tcl bash openssl
# Fri, 18 Mar 2022 14:46:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 18 Mar 2022 14:46:53 GMT
ENV NICK=
# Fri, 18 Mar 2022 14:46:54 GMT
ENV SERVER=
# Fri, 18 Mar 2022 14:46:55 GMT
ENV LISTEN=3333
# Fri, 18 Mar 2022 14:46:56 GMT
ENV OWNER=
# Fri, 18 Mar 2022 14:46:57 GMT
ENV USERFILE=eggdrop.user
# Fri, 18 Mar 2022 14:46:58 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 18 Mar 2022 14:46:59 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 18 Mar 2022 14:47:00 GMT
EXPOSE 3333
# Fri, 18 Mar 2022 14:47:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Fri, 18 Mar 2022 14:47:03 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 18 Mar 2022 14:47:03 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 18 Mar 2022 14:47:04 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb7d5a2ca34099ee59f1fe9cf95cdebe5333240fc3fcc85b1f87385f2009182`  
		Last Modified: Fri, 18 Mar 2022 14:47:27 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f63adfc43a1a5c75fc2ae2f1ef9a21be6ea3cd3f23e49b1f5b848538d4d65a1`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 10.5 KB (10479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a4fe92bba72599e1e2ff73684c341d4588bde58f8ac95df4d2ca47f0edb58c`  
		Last Modified: Fri, 18 Mar 2022 14:47:25 GMT  
		Size: 2.8 MB (2752210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d7283084533cfc36469ab71ac7cbdf4d43225dc13dcdd05f00c69c6a28ebb7`  
		Last Modified: Fri, 18 Mar 2022 14:47:25 GMT  
		Size: 2.7 MB (2719723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea66aaf353f32b17778bb9aa25dc17273e21a3b37ddf4315552269025569cee`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba34823c5a1a78d76f8ddcd7a709dc0f6c55f23cab8203d64ea6c3a79b51d3`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.2`

```console
$ docker pull eggdrop@sha256:1fa1f45990945b00fdf398a825c1868736b37dd0605affcd075a51a1f76b1ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9.2` - linux; amd64

```console
$ docker pull eggdrop@sha256:a9b09dad37a7d351adf38d5a3235c12af1ed3564b73aac2ba748d58e345376b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8282046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9dd1bbf14a48744b1dec02b68a901079951585fe36d1e87218895d262d98516`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:05:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 19 Mar 2022 03:05:37 GMT
RUN adduser -S eggdrop
# Sat, 19 Mar 2022 03:05:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 03:05:39 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 19 Mar 2022 03:07:15 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 19 Mar 2022 03:07:15 GMT
ENV NICK=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV SERVER=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV LISTEN=3333
# Sat, 19 Mar 2022 03:07:15 GMT
ENV OWNER=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV USERFILE=eggdrop.user
# Sat, 19 Mar 2022 03:07:15 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 19 Mar 2022 03:07:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 19 Mar 2022 03:07:15 GMT
EXPOSE 3333
# Sat, 19 Mar 2022 03:07:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 19 Mar 2022 03:07:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 19 Mar 2022 03:07:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 19 Mar 2022 03:07:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cef478d9d2e17c2069b3b787f432f66639b715bbf9fc9be426ae6aa3ef59c2f`  
		Last Modified: Sat, 19 Mar 2022 03:07:41 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389bcdf8f16100f8d9c2358a3cf00ce0b5cd27b98ddf4951213e6b6349c73c6b`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 10.7 KB (10701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f092587418f14c475253126c75b2c2f98611f67d66a9df545bdfcd79f63ecb54`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 2.7 MB (2725676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a220e2a1485d9064ab75a27e36c756f0dc76c045749f01bf95fbf2d4b13398`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 2.7 MB (2724694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdb7391b21cc18aa21e66bdbaf6dfa1f09c6008cf67bc5e6967caff6a6fb038`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6526ffbb05a9b20439dce8e5c1749c8e6b36f1de10ae3c4570ea9c18821e088`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.2` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:122bb0227f48ef8fe35ba5812cb8958afb24465ccfd5c7ac68be28f5a63b204d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7978193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a651c413330366ccced3e0f0ef84e38f1bbfa847251f4d46b94f11379d9dad`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:15:44 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Mar 2022 15:15:45 GMT
RUN adduser -S eggdrop
# Thu, 17 Mar 2022 15:15:47 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Mar 2022 15:15:50 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Mar 2022 15:18:23 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Mar 2022 15:18:24 GMT
ENV NICK=
# Thu, 17 Mar 2022 15:18:24 GMT
ENV SERVER=
# Thu, 17 Mar 2022 15:18:24 GMT
ENV LISTEN=3333
# Thu, 17 Mar 2022 15:18:25 GMT
ENV OWNER=
# Thu, 17 Mar 2022 15:18:25 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Mar 2022 15:18:26 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Mar 2022 15:18:26 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Mar 2022 15:18:26 GMT
EXPOSE 3333
# Thu, 17 Mar 2022 15:18:27 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 17 Mar 2022 15:18:27 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Mar 2022 15:18:28 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Mar 2022 15:18:28 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1e510cf840340b9c34cfa14cc3fc7a832572443f28af0d2c63cf30dec078`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cb7fa74ab74933c3d0f5a43b2b2e0f5cb4332ad9e0f3d558b3bc296e438dad`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 10.4 KB (10402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce325b134d392e303241c318e8f3927c9fff71180df7ab82013df55879374047`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 2.7 MB (2652778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12377e78aa28c481d5f31d50a704199e7a8ece0d814e51692670d1dfcdf210`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 2.7 MB (2683288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0311035445d15202ed8f1d5d853071ea99fcd4919d47c93ffe8b3dd72cf901`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df94df2aefc0ab73ed8cdc9d8e440c91a76a178bc7a7e93c2564e770d5a22bb`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.2` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c238c47c3943e2433b9b4b521d1216015d5382efcfd6b2f205b2b3811e578b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8205326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3360c1069756788284a40b6b4d98d5c5524e0831045b8c9f7fc6c4390ca8c7d`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:45:12 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 18 Mar 2022 14:45:13 GMT
RUN adduser -S eggdrop
# Fri, 18 Mar 2022 14:45:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 18 Mar 2022 14:45:16 GMT
RUN apk add --no-cache tcl bash openssl
# Fri, 18 Mar 2022 14:46:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 18 Mar 2022 14:46:53 GMT
ENV NICK=
# Fri, 18 Mar 2022 14:46:54 GMT
ENV SERVER=
# Fri, 18 Mar 2022 14:46:55 GMT
ENV LISTEN=3333
# Fri, 18 Mar 2022 14:46:56 GMT
ENV OWNER=
# Fri, 18 Mar 2022 14:46:57 GMT
ENV USERFILE=eggdrop.user
# Fri, 18 Mar 2022 14:46:58 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 18 Mar 2022 14:46:59 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 18 Mar 2022 14:47:00 GMT
EXPOSE 3333
# Fri, 18 Mar 2022 14:47:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Fri, 18 Mar 2022 14:47:03 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 18 Mar 2022 14:47:03 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 18 Mar 2022 14:47:04 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb7d5a2ca34099ee59f1fe9cf95cdebe5333240fc3fcc85b1f87385f2009182`  
		Last Modified: Fri, 18 Mar 2022 14:47:27 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f63adfc43a1a5c75fc2ae2f1ef9a21be6ea3cd3f23e49b1f5b848538d4d65a1`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 10.5 KB (10479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a4fe92bba72599e1e2ff73684c341d4588bde58f8ac95df4d2ca47f0edb58c`  
		Last Modified: Fri, 18 Mar 2022 14:47:25 GMT  
		Size: 2.8 MB (2752210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d7283084533cfc36469ab71ac7cbdf4d43225dc13dcdd05f00c69c6a28ebb7`  
		Last Modified: Fri, 18 Mar 2022 14:47:25 GMT  
		Size: 2.7 MB (2719723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea66aaf353f32b17778bb9aa25dc17273e21a3b37ddf4315552269025569cee`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba34823c5a1a78d76f8ddcd7a709dc0f6c55f23cab8203d64ea6c3a79b51d3`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:45bee3e2b094ddbdbb0c5a9f2e1f192549a4fc0eb5e5cf076ff8b1fb4bc01cd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:c4fc120464aba7fe99193b5247958596da13a360d55b5bd6eed2738fb92ef53e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39769193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd7dd5e41102214aad3e4adcd630b8481b65eda8256ff4a2a27c41d08f0a5c44`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:49:34 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Mar 2022 08:49:35 GMT
RUN adduser -S eggdrop
# Thu, 17 Mar 2022 08:49:36 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Mar 2022 08:49:36 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Thu, 17 Mar 2022 08:49:36 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Thu, 17 Mar 2022 08:49:37 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 17 Mar 2022 08:54:00 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Mar 2022 08:54:00 GMT
ENV NICK=
# Thu, 17 Mar 2022 08:54:00 GMT
ENV SERVER=
# Thu, 17 Mar 2022 08:54:00 GMT
ENV LISTEN=3333
# Thu, 17 Mar 2022 08:54:00 GMT
ENV OWNER=
# Thu, 17 Mar 2022 08:54:01 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Mar 2022 08:54:01 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Mar 2022 08:54:01 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Mar 2022 08:54:01 GMT
EXPOSE 3333
# Thu, 17 Mar 2022 08:54:01 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Thu, 17 Mar 2022 08:54:01 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Mar 2022 08:54:01 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Mar 2022 08:54:01 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaa7543d03648683193902d678c5004ad3d5bf64914ea4b51de9cf5efcc4ae1`  
		Last Modified: Thu, 17 Mar 2022 08:54:25 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93422708359b63ffb56d0dc058277b02370ae9aa76ba0608870d2255cc5fa4d4`  
		Last Modified: Thu, 17 Mar 2022 08:54:23 GMT  
		Size: 11.0 KB (10953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11262aa65548d6c137c6daa98100b81c4a11c3b4004dfec0607cfb48ca6d400`  
		Last Modified: Thu, 17 Mar 2022 08:54:23 GMT  
		Size: 1.1 MB (1089648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c53473dbd628ef0d26779b6bf1a855b6779cd3e74891e7474fb5d1e047e714`  
		Last Modified: Thu, 17 Mar 2022 08:54:29 GMT  
		Size: 35.9 MB (35852112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b7c14e7ff48f3ca1a7a7b4f27a750eaa6af963b52ea18c7bb1e885d2a93cc1`  
		Last Modified: Thu, 17 Mar 2022 08:54:23 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1de2314ae566844c0aa5483e9cf609762dd74c6be08814b61e23e590c00a9c`  
		Last Modified: Thu, 17 Mar 2022 08:54:23 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:24d74c58a4f0284360af9c6e90eac4a24bc33243f7a37eb2c33751412fe57b9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39168942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f9a53a52110af0ab7d4e6b839b07dcfe527eb869a861240cc09c9ab5aa33e09`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 05:28:28 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Mar 2022 05:28:30 GMT
RUN adduser -S eggdrop
# Thu, 17 Mar 2022 05:28:32 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Mar 2022 05:28:33 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Thu, 17 Mar 2022 05:28:33 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Thu, 17 Mar 2022 05:28:35 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 17 Mar 2022 05:38:44 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Mar 2022 05:38:45 GMT
ENV NICK=
# Thu, 17 Mar 2022 05:38:46 GMT
ENV SERVER=
# Thu, 17 Mar 2022 05:38:46 GMT
ENV LISTEN=3333
# Thu, 17 Mar 2022 05:38:46 GMT
ENV OWNER=
# Thu, 17 Mar 2022 05:38:47 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Mar 2022 05:38:47 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Mar 2022 05:38:48 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Mar 2022 05:38:48 GMT
EXPOSE 3333
# Thu, 17 Mar 2022 05:38:49 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Thu, 17 Mar 2022 05:38:49 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Mar 2022 05:38:49 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Mar 2022 05:38:50 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b68efa6a1997325a5ae45e779e3a144141f203b55e7238ffdf2a34e7054a53`  
		Last Modified: Thu, 17 Mar 2022 05:39:47 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edf584a6d64b54a3f3ec767c0e0998424b3d5e97db05836574741e8de66c09`  
		Last Modified: Thu, 17 Mar 2022 05:39:45 GMT  
		Size: 10.7 KB (10663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0864307a79503dd64dc6fe912a977e1f5db6f1cb81d972b229d718aa4d5adb`  
		Last Modified: Thu, 17 Mar 2022 05:39:46 GMT  
		Size: 1.0 MB (1032374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1248ce657c21528dfe5b7bbcde4402928c58776f5d5f78e9d4d009c95cad32a9`  
		Last Modified: Thu, 17 Mar 2022 05:40:10 GMT  
		Size: 35.5 MB (35497075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c9b64037e1a3a6d789a32a21f951a6970d05d37e8c73cac695c5a446d8278`  
		Last Modified: Thu, 17 Mar 2022 05:39:45 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306d1e09adf54334b46c6ceed7b7b9f39b6c7b659b494314db12588a00ac8a5e`  
		Last Modified: Thu, 17 Mar 2022 05:39:45 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c76047585ccd86aca955c0e6bc42a3411c75416e2852eba414f25b1390f333b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39838487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e456e828f6873a23e76e6c5f10ef1a9bca164127e919c17ad41e52a79036e1d`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 06:48:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Mar 2022 06:48:57 GMT
RUN adduser -S eggdrop
# Thu, 17 Mar 2022 06:48:59 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Mar 2022 06:48:59 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Thu, 17 Mar 2022 06:49:00 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Thu, 17 Mar 2022 06:49:01 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 17 Mar 2022 06:53:49 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Mar 2022 06:53:49 GMT
ENV NICK=
# Thu, 17 Mar 2022 06:53:50 GMT
ENV SERVER=
# Thu, 17 Mar 2022 06:53:51 GMT
ENV LISTEN=3333
# Thu, 17 Mar 2022 06:53:52 GMT
ENV OWNER=
# Thu, 17 Mar 2022 06:53:53 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Mar 2022 06:53:54 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Mar 2022 06:53:55 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Mar 2022 06:53:56 GMT
EXPOSE 3333
# Thu, 17 Mar 2022 06:53:58 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Thu, 17 Mar 2022 06:53:59 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Mar 2022 06:53:59 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Mar 2022 06:54:00 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49fc19ed302ad49df1bc3ac497157d115745e9ed6cf702ccc18ab6489dc1d8e`  
		Last Modified: Thu, 17 Mar 2022 06:54:29 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa846be34df0900bdf403c5c5f07bbd0a2fb3585e0eecd8b6b4a760a75448ba8`  
		Last Modified: Thu, 17 Mar 2022 06:54:27 GMT  
		Size: 10.7 KB (10673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21934b1a15b075daf87e07d881760d39a0a6f0cd143cff973fa2a64cc382f1a8`  
		Last Modified: Thu, 17 Mar 2022 06:54:27 GMT  
		Size: 1.1 MB (1087192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab5070e3f7ae4612ff31aa43e7241f726f60ca30e131e3dd5a2b0c946b5e485`  
		Last Modified: Thu, 17 Mar 2022 06:54:32 GMT  
		Size: 36.0 MB (36021980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fe8df42b6a33034dff05c622b4c544c0d759c6b66bd6a320a418cf441c6b3`  
		Last Modified: Thu, 17 Mar 2022 06:54:27 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dc54c4e71ff38f1db4507e6c33a3ce6f4707945d7ac42d1eca7708011f86af`  
		Last Modified: Thu, 17 Mar 2022 06:54:27 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:1fa1f45990945b00fdf398a825c1868736b37dd0605affcd075a51a1f76b1ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:a9b09dad37a7d351adf38d5a3235c12af1ed3564b73aac2ba748d58e345376b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8282046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9dd1bbf14a48744b1dec02b68a901079951585fe36d1e87218895d262d98516`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:05:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 19 Mar 2022 03:05:37 GMT
RUN adduser -S eggdrop
# Sat, 19 Mar 2022 03:05:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 03:05:39 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 19 Mar 2022 03:07:15 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 19 Mar 2022 03:07:15 GMT
ENV NICK=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV SERVER=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV LISTEN=3333
# Sat, 19 Mar 2022 03:07:15 GMT
ENV OWNER=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV USERFILE=eggdrop.user
# Sat, 19 Mar 2022 03:07:15 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 19 Mar 2022 03:07:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 19 Mar 2022 03:07:15 GMT
EXPOSE 3333
# Sat, 19 Mar 2022 03:07:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 19 Mar 2022 03:07:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 19 Mar 2022 03:07:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 19 Mar 2022 03:07:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cef478d9d2e17c2069b3b787f432f66639b715bbf9fc9be426ae6aa3ef59c2f`  
		Last Modified: Sat, 19 Mar 2022 03:07:41 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389bcdf8f16100f8d9c2358a3cf00ce0b5cd27b98ddf4951213e6b6349c73c6b`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 10.7 KB (10701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f092587418f14c475253126c75b2c2f98611f67d66a9df545bdfcd79f63ecb54`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 2.7 MB (2725676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a220e2a1485d9064ab75a27e36c756f0dc76c045749f01bf95fbf2d4b13398`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 2.7 MB (2724694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdb7391b21cc18aa21e66bdbaf6dfa1f09c6008cf67bc5e6967caff6a6fb038`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6526ffbb05a9b20439dce8e5c1749c8e6b36f1de10ae3c4570ea9c18821e088`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:122bb0227f48ef8fe35ba5812cb8958afb24465ccfd5c7ac68be28f5a63b204d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7978193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a651c413330366ccced3e0f0ef84e38f1bbfa847251f4d46b94f11379d9dad`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:15:44 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Mar 2022 15:15:45 GMT
RUN adduser -S eggdrop
# Thu, 17 Mar 2022 15:15:47 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Mar 2022 15:15:50 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Mar 2022 15:18:23 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Mar 2022 15:18:24 GMT
ENV NICK=
# Thu, 17 Mar 2022 15:18:24 GMT
ENV SERVER=
# Thu, 17 Mar 2022 15:18:24 GMT
ENV LISTEN=3333
# Thu, 17 Mar 2022 15:18:25 GMT
ENV OWNER=
# Thu, 17 Mar 2022 15:18:25 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Mar 2022 15:18:26 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Mar 2022 15:18:26 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Mar 2022 15:18:26 GMT
EXPOSE 3333
# Thu, 17 Mar 2022 15:18:27 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 17 Mar 2022 15:18:27 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Mar 2022 15:18:28 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Mar 2022 15:18:28 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1e510cf840340b9c34cfa14cc3fc7a832572443f28af0d2c63cf30dec078`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cb7fa74ab74933c3d0f5a43b2b2e0f5cb4332ad9e0f3d558b3bc296e438dad`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 10.4 KB (10402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce325b134d392e303241c318e8f3927c9fff71180df7ab82013df55879374047`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 2.7 MB (2652778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12377e78aa28c481d5f31d50a704199e7a8ece0d814e51692670d1dfcdf210`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 2.7 MB (2683288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0311035445d15202ed8f1d5d853071ea99fcd4919d47c93ffe8b3dd72cf901`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df94df2aefc0ab73ed8cdc9d8e440c91a76a178bc7a7e93c2564e770d5a22bb`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c238c47c3943e2433b9b4b521d1216015d5382efcfd6b2f205b2b3811e578b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8205326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3360c1069756788284a40b6b4d98d5c5524e0831045b8c9f7fc6c4390ca8c7d`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:45:12 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 18 Mar 2022 14:45:13 GMT
RUN adduser -S eggdrop
# Fri, 18 Mar 2022 14:45:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 18 Mar 2022 14:45:16 GMT
RUN apk add --no-cache tcl bash openssl
# Fri, 18 Mar 2022 14:46:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 18 Mar 2022 14:46:53 GMT
ENV NICK=
# Fri, 18 Mar 2022 14:46:54 GMT
ENV SERVER=
# Fri, 18 Mar 2022 14:46:55 GMT
ENV LISTEN=3333
# Fri, 18 Mar 2022 14:46:56 GMT
ENV OWNER=
# Fri, 18 Mar 2022 14:46:57 GMT
ENV USERFILE=eggdrop.user
# Fri, 18 Mar 2022 14:46:58 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 18 Mar 2022 14:46:59 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 18 Mar 2022 14:47:00 GMT
EXPOSE 3333
# Fri, 18 Mar 2022 14:47:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Fri, 18 Mar 2022 14:47:03 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 18 Mar 2022 14:47:03 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 18 Mar 2022 14:47:04 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb7d5a2ca34099ee59f1fe9cf95cdebe5333240fc3fcc85b1f87385f2009182`  
		Last Modified: Fri, 18 Mar 2022 14:47:27 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f63adfc43a1a5c75fc2ae2f1ef9a21be6ea3cd3f23e49b1f5b848538d4d65a1`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 10.5 KB (10479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a4fe92bba72599e1e2ff73684c341d4588bde58f8ac95df4d2ca47f0edb58c`  
		Last Modified: Fri, 18 Mar 2022 14:47:25 GMT  
		Size: 2.8 MB (2752210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d7283084533cfc36469ab71ac7cbdf4d43225dc13dcdd05f00c69c6a28ebb7`  
		Last Modified: Fri, 18 Mar 2022 14:47:25 GMT  
		Size: 2.7 MB (2719723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea66aaf353f32b17778bb9aa25dc17273e21a3b37ddf4315552269025569cee`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba34823c5a1a78d76f8ddcd7a709dc0f6c55f23cab8203d64ea6c3a79b51d3`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:1fa1f45990945b00fdf398a825c1868736b37dd0605affcd075a51a1f76b1ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:a9b09dad37a7d351adf38d5a3235c12af1ed3564b73aac2ba748d58e345376b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8282046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9dd1bbf14a48744b1dec02b68a901079951585fe36d1e87218895d262d98516`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:05:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 19 Mar 2022 03:05:37 GMT
RUN adduser -S eggdrop
# Sat, 19 Mar 2022 03:05:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 03:05:39 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 19 Mar 2022 03:07:15 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 19 Mar 2022 03:07:15 GMT
ENV NICK=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV SERVER=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV LISTEN=3333
# Sat, 19 Mar 2022 03:07:15 GMT
ENV OWNER=
# Sat, 19 Mar 2022 03:07:15 GMT
ENV USERFILE=eggdrop.user
# Sat, 19 Mar 2022 03:07:15 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 19 Mar 2022 03:07:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 19 Mar 2022 03:07:15 GMT
EXPOSE 3333
# Sat, 19 Mar 2022 03:07:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 19 Mar 2022 03:07:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 19 Mar 2022 03:07:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 19 Mar 2022 03:07:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cef478d9d2e17c2069b3b787f432f66639b715bbf9fc9be426ae6aa3ef59c2f`  
		Last Modified: Sat, 19 Mar 2022 03:07:41 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389bcdf8f16100f8d9c2358a3cf00ce0b5cd27b98ddf4951213e6b6349c73c6b`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 10.7 KB (10701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f092587418f14c475253126c75b2c2f98611f67d66a9df545bdfcd79f63ecb54`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 2.7 MB (2725676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a220e2a1485d9064ab75a27e36c756f0dc76c045749f01bf95fbf2d4b13398`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 2.7 MB (2724694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdb7391b21cc18aa21e66bdbaf6dfa1f09c6008cf67bc5e6967caff6a6fb038`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6526ffbb05a9b20439dce8e5c1749c8e6b36f1de10ae3c4570ea9c18821e088`  
		Last Modified: Sat, 19 Mar 2022 03:07:39 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:122bb0227f48ef8fe35ba5812cb8958afb24465ccfd5c7ac68be28f5a63b204d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7978193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a651c413330366ccced3e0f0ef84e38f1bbfa847251f4d46b94f11379d9dad`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:15:44 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Mar 2022 15:15:45 GMT
RUN adduser -S eggdrop
# Thu, 17 Mar 2022 15:15:47 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Mar 2022 15:15:50 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Mar 2022 15:18:23 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Mar 2022 15:18:24 GMT
ENV NICK=
# Thu, 17 Mar 2022 15:18:24 GMT
ENV SERVER=
# Thu, 17 Mar 2022 15:18:24 GMT
ENV LISTEN=3333
# Thu, 17 Mar 2022 15:18:25 GMT
ENV OWNER=
# Thu, 17 Mar 2022 15:18:25 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Mar 2022 15:18:26 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Mar 2022 15:18:26 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Mar 2022 15:18:26 GMT
EXPOSE 3333
# Thu, 17 Mar 2022 15:18:27 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 17 Mar 2022 15:18:27 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Mar 2022 15:18:28 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Mar 2022 15:18:28 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1e510cf840340b9c34cfa14cc3fc7a832572443f28af0d2c63cf30dec078`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cb7fa74ab74933c3d0f5a43b2b2e0f5cb4332ad9e0f3d558b3bc296e438dad`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 10.4 KB (10402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce325b134d392e303241c318e8f3927c9fff71180df7ab82013df55879374047`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 2.7 MB (2652778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12377e78aa28c481d5f31d50a704199e7a8ece0d814e51692670d1dfcdf210`  
		Last Modified: Thu, 17 Mar 2022 15:19:16 GMT  
		Size: 2.7 MB (2683288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0311035445d15202ed8f1d5d853071ea99fcd4919d47c93ffe8b3dd72cf901`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df94df2aefc0ab73ed8cdc9d8e440c91a76a178bc7a7e93c2564e770d5a22bb`  
		Last Modified: Thu, 17 Mar 2022 15:19:14 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c238c47c3943e2433b9b4b521d1216015d5382efcfd6b2f205b2b3811e578b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8205326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3360c1069756788284a40b6b4d98d5c5524e0831045b8c9f7fc6c4390ca8c7d`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:45:12 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 18 Mar 2022 14:45:13 GMT
RUN adduser -S eggdrop
# Fri, 18 Mar 2022 14:45:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 18 Mar 2022 14:45:16 GMT
RUN apk add --no-cache tcl bash openssl
# Fri, 18 Mar 2022 14:46:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.2.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.2.tar.gz.asc eggdrop-1.9.2.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.2.tar.gz.asc   && tar -zxvf eggdrop-1.9.2.tar.gz   && rm eggdrop-1.9.2.tar.gz   && ( cd eggdrop-1.9.2     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.2   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 18 Mar 2022 14:46:53 GMT
ENV NICK=
# Fri, 18 Mar 2022 14:46:54 GMT
ENV SERVER=
# Fri, 18 Mar 2022 14:46:55 GMT
ENV LISTEN=3333
# Fri, 18 Mar 2022 14:46:56 GMT
ENV OWNER=
# Fri, 18 Mar 2022 14:46:57 GMT
ENV USERFILE=eggdrop.user
# Fri, 18 Mar 2022 14:46:58 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 18 Mar 2022 14:46:59 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 18 Mar 2022 14:47:00 GMT
EXPOSE 3333
# Fri, 18 Mar 2022 14:47:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Fri, 18 Mar 2022 14:47:03 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 18 Mar 2022 14:47:03 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 18 Mar 2022 14:47:04 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb7d5a2ca34099ee59f1fe9cf95cdebe5333240fc3fcc85b1f87385f2009182`  
		Last Modified: Fri, 18 Mar 2022 14:47:27 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f63adfc43a1a5c75fc2ae2f1ef9a21be6ea3cd3f23e49b1f5b848538d4d65a1`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 10.5 KB (10479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a4fe92bba72599e1e2ff73684c341d4588bde58f8ac95df4d2ca47f0edb58c`  
		Last Modified: Fri, 18 Mar 2022 14:47:25 GMT  
		Size: 2.8 MB (2752210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d7283084533cfc36469ab71ac7cbdf4d43225dc13dcdd05f00c69c6a28ebb7`  
		Last Modified: Fri, 18 Mar 2022 14:47:25 GMT  
		Size: 2.7 MB (2719723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea66aaf353f32b17778bb9aa25dc17273e21a3b37ddf4315552269025569cee`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba34823c5a1a78d76f8ddcd7a709dc0f6c55f23cab8203d64ea6c3a79b51d3`  
		Last Modified: Fri, 18 Mar 2022 14:47:24 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
