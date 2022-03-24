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
$ docker pull eggdrop@sha256:7495b409663c6888cd77a8e0d11b40a0cc94cc0f3ae51ac7906a30e82dd69fbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:6dc7f987a543bd5af3b3630819b63c393f4b50718993b1e83d83cb922f07b5b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39769225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca91a541c054b2e7ce3e6a9c5a8538842c22be50b07e940b6c413c00c1fad5e`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 18:00:24 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 23 Mar 2022 18:00:24 GMT
RUN adduser -S eggdrop
# Wed, 23 Mar 2022 18:00:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 23 Mar 2022 18:00:25 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Wed, 23 Mar 2022 18:00:25 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Wed, 23 Mar 2022 18:00:26 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 23 Mar 2022 18:04:14 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 23 Mar 2022 18:04:14 GMT
ENV NICK=
# Wed, 23 Mar 2022 18:04:14 GMT
ENV SERVER=
# Wed, 23 Mar 2022 18:04:15 GMT
ENV LISTEN=3333
# Wed, 23 Mar 2022 18:04:15 GMT
ENV OWNER=
# Wed, 23 Mar 2022 18:04:15 GMT
ENV USERFILE=eggdrop.user
# Wed, 23 Mar 2022 18:04:15 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 23 Mar 2022 18:04:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 23 Mar 2022 18:04:15 GMT
EXPOSE 3333
# Wed, 23 Mar 2022 18:04:15 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Wed, 23 Mar 2022 18:04:15 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 23 Mar 2022 18:04:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 23 Mar 2022 18:04:15 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255d707abd67e2212c0fc03a42dec647e762d447679bc356b91ee54e0d6a2279`  
		Last Modified: Wed, 23 Mar 2022 18:04:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14c34e2c83cb8386f15d815f78551415b0902c87b29d55d6cf6d927d447e905`  
		Last Modified: Wed, 23 Mar 2022 18:04:43 GMT  
		Size: 11.0 KB (10951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5822447b6736a6926d59167c3028d4b67485d04cb49b0d51c1f9f9a56de5a2d`  
		Last Modified: Wed, 23 Mar 2022 18:04:44 GMT  
		Size: 1.1 MB (1089640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd5c879203d7fc23ea2576276c36cb94b1eb1bc2145bb9ab0604d2ce145fac6`  
		Last Modified: Wed, 23 Mar 2022 18:04:49 GMT  
		Size: 35.9 MB (35852104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a15c9f725267f25678469c1126908993d96012c017bdc13a955eb42a79674`  
		Last Modified: Wed, 23 Mar 2022 18:04:43 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7d93b5f91d9637631b5c443044c61c7f7985d546ad0b9ed44d60dbc72c2222`  
		Last Modified: Wed, 23 Mar 2022 18:04:43 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:27f37eb9c752253ee4bde14b7a08dbdca44b665dcc201c9557263b8de458d7e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39168806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b56174b0f105dd4699df029abe3f520a415e7da53575c8a72475addaa613fa4`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 23 Mar 2022 15:49:35 GMT
ADD file:fd7f6da4a48df653ae6dd18e6d5959008daf5ce429845c974982dc7d213342d9 in / 
# Wed, 23 Mar 2022 15:49:35 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:06:53 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 23 Mar 2022 19:06:55 GMT
RUN adduser -S eggdrop
# Wed, 23 Mar 2022 19:06:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 23 Mar 2022 19:06:58 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Wed, 23 Mar 2022 19:06:58 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Wed, 23 Mar 2022 19:07:00 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 23 Mar 2022 19:17:14 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 23 Mar 2022 19:17:15 GMT
ENV NICK=
# Wed, 23 Mar 2022 19:17:15 GMT
ENV SERVER=
# Wed, 23 Mar 2022 19:17:16 GMT
ENV LISTEN=3333
# Wed, 23 Mar 2022 19:17:16 GMT
ENV OWNER=
# Wed, 23 Mar 2022 19:17:16 GMT
ENV USERFILE=eggdrop.user
# Wed, 23 Mar 2022 19:17:17 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 23 Mar 2022 19:17:17 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 23 Mar 2022 19:17:18 GMT
EXPOSE 3333
# Wed, 23 Mar 2022 19:17:18 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Wed, 23 Mar 2022 19:17:19 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 23 Mar 2022 19:17:19 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 23 Mar 2022 19:17:20 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4e012d7cd81aa4570d9d209a75131b32f34a3533d5d449d23fd875513922588e`  
		Last Modified: Wed, 23 Mar 2022 15:51:07 GMT  
		Size: 2.6 MB (2624816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965e56d6e8a96c88d0f2e343e906f0f47708d69c6c7ba96170539e225d9a1327`  
		Last Modified: Wed, 23 Mar 2022 19:18:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9e393b2f7b36b3a8f977f997113293e5cc6eb8be0bc20f33da61dedb0cb983`  
		Last Modified: Wed, 23 Mar 2022 19:18:10 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13eb94631bb879fe11051546544fe4d36f813d5d6a07d14a2979b6f391888c2c`  
		Last Modified: Wed, 23 Mar 2022 19:18:11 GMT  
		Size: 1.0 MB (1032367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d923ce278658b2f5f2cb82a065495eb0dca24b60f271eb0e59e0c668ea11c311`  
		Last Modified: Wed, 23 Mar 2022 19:18:33 GMT  
		Size: 35.5 MB (35497119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8befdb0d8e2a12810a2081e45a6695415d67b868ece4ef870717113a0e265967`  
		Last Modified: Wed, 23 Mar 2022 19:18:10 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a7e899a3c002c1efb9193807175661e713ea81fbf230c1725f3494bef21c9f`  
		Last Modified: Wed, 23 Mar 2022 19:18:10 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:d0a929ef427192b69a8d46b58c69795d66a2bb3d576fa139e5f67df6ac419cd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39838531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:479af0ffbdfb008f646b611a5ca182fd0afbe940474b3034e6877bbaf64f9bcf`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:09:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 24 Mar 2022 05:09:46 GMT
RUN adduser -S eggdrop
# Thu, 24 Mar 2022 05:09:47 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 24 Mar 2022 05:09:48 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Thu, 24 Mar 2022 05:09:49 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Thu, 24 Mar 2022 05:09:50 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 24 Mar 2022 05:14:25 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 24 Mar 2022 05:14:25 GMT
ENV NICK=
# Thu, 24 Mar 2022 05:14:26 GMT
ENV SERVER=
# Thu, 24 Mar 2022 05:14:27 GMT
ENV LISTEN=3333
# Thu, 24 Mar 2022 05:14:28 GMT
ENV OWNER=
# Thu, 24 Mar 2022 05:14:29 GMT
ENV USERFILE=eggdrop.user
# Thu, 24 Mar 2022 05:14:30 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 24 Mar 2022 05:14:31 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 24 Mar 2022 05:14:32 GMT
EXPOSE 3333
# Thu, 24 Mar 2022 05:14:34 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Thu, 24 Mar 2022 05:14:35 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 24 Mar 2022 05:14:35 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 24 Mar 2022 05:14:36 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92d91ef5604aa6e111155577809aab2aced2a26845776cd2c773c5c98e79a1`  
		Last Modified: Thu, 24 Mar 2022 05:15:02 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b03347ecda5c13c2c0f9eb606388d846582e9f73524377dfac6903c60517e21`  
		Last Modified: Thu, 24 Mar 2022 05:15:00 GMT  
		Size: 10.7 KB (10671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a899e7ef52155c77836fd4652ba64c5a48bf1103cf17dd758252a9427bfd06a9`  
		Last Modified: Thu, 24 Mar 2022 05:15:00 GMT  
		Size: 1.1 MB (1087185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc2e3fd0cd7ed5aeeaf0b3e4064f5a3f9085ed3e7592185f1b506e1ed113086`  
		Last Modified: Thu, 24 Mar 2022 05:15:06 GMT  
		Size: 36.0 MB (36022125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027493c578e97be9ca98c58e40135165aac7e7e0ce1ac9ede0702c72517253d`  
		Last Modified: Thu, 24 Mar 2022 05:15:00 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38dca678f81b40c9820012fc3f8f4454f84651583820ff9c2ca3b8816949584`  
		Last Modified: Thu, 24 Mar 2022 05:15:00 GMT  
		Size: 703.0 B  
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
