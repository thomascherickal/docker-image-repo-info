<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.5`](#eggdrop195)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:3d23b6c36a7a3c389ab7d65c8d9408083d7513e6e9d1e7eb9531001e4dfdd07a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:fbb76e4f3fd2ee92563febb33b858d7bfc23e8a4ae90e77a0e6f065d7cd63f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11727481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5a2e0d5610d91f6e6b5b086fbc0a0e1f8413c9c9c52d6b8b4818b903ea7b42`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:42:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 15 Jun 2023 04:42:23 GMT
RUN adduser -S eggdrop
# Thu, 15 Jun 2023 04:42:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 15 Jun 2023 04:42:25 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 15 Jun 2023 04:46:22 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 15 Jun 2023 04:46:22 GMT
ENV NICK=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV SERVER=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV LISTEN=3333
# Thu, 15 Jun 2023 04:46:23 GMT
ENV OWNER=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV USERFILE=eggdrop.user
# Thu, 15 Jun 2023 04:46:23 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 15 Jun 2023 04:46:23 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 15 Jun 2023 04:46:23 GMT
EXPOSE 3333
# Thu, 15 Jun 2023 04:46:23 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 15 Jun 2023 04:46:23 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 15 Jun 2023 04:46:23 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 15 Jun 2023 04:46:23 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d216fc621c25522e777539ef90b86c566f8e186359154b2bfab46d0c793b0c9b`  
		Last Modified: Thu, 15 Jun 2023 04:46:47 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a5e16c27c10687f1f1b429526c75e1707ab0ea50ce602df684dda6b331f42`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 10.9 KB (10941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dc4cfb0d27369f3d3e88018e01f830d17dbdebe4b91ab24ccdbd3d6ba9d66a`  
		Last Modified: Thu, 15 Jun 2023 04:46:46 GMT  
		Size: 2.8 MB (2758065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8419a4c44d78db125dcd808f917e289ee923e5ee4b68758d01a3504a4745766d`  
		Last Modified: Thu, 15 Jun 2023 04:46:46 GMT  
		Size: 6.1 MB (6146999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c25e7ab8efa8ccdd354e83f46706704a0198eba17ccbf4964a827e3c8e7ff8a`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ebad7fb733ee98c26ad75a26d0b1b1d36e178e165faf0ed6a5fc8be1aaed6c`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:b8f18f32c6f50d3d622b687a62a98063626c1ebaad90b88615b01cce14c94f6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11363954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1faba54e962f458cbc99783a3c0429a3bdf9b487dfd87861c7e32eaaf592ac`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:28 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
# Wed, 14 Jun 2023 18:49:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 19:50:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 19:50:57 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 19:51:00 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 19:51:03 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 14 Jun 2023 19:56:08 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 19:56:08 GMT
ENV NICK=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV SERVER=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 19:56:09 GMT
ENV OWNER=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 19:56:09 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 19:56:09 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 19:56:09 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 19:56:09 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 19:56:09 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 19:56:09 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 19:56:09 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59edb5f625f9baba9a7ea41967538ecb65f8f3a2c21dbaac52c1cebdda71f4c5`  
		Last Modified: Wed, 14 Jun 2023 19:56:37 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d91c589e5b4c6197aed20876f69cbd4e6c2b756d05e459b7ac6bbcabe136c7`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 10.6 KB (10631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fdffc7323d45dd58aa0359aab7e2d9f9f375fddb9958fcd64fd770c94daf83`  
		Last Modified: Wed, 14 Jun 2023 19:56:36 GMT  
		Size: 2.7 MB (2679963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d7b4abdc31f67a9db93623090b78267d3fea57aef5ce525ffa72866261ccd`  
		Last Modified: Wed, 14 Jun 2023 19:56:37 GMT  
		Size: 6.1 MB (6053977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114272a2dc638a3349674767d3512c750bc67c2aa58ab072006c0c343c129aa8`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4afb0fc779b33a25070697e8911beeae28c81d7400a42941eee76a2e95ba1`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:30e1a07d96fd6931347842b9e336e3406c69a22af5a30ee3a6c6eede82c759db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11686144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95261f7f791cadf51418239f765292865cfdb39a9c8ac55c55c2addba62a289f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:51:05 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 22:51:05 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 22:51:06 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 22:51:08 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 14 Jun 2023 22:54:57 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 22:54:57 GMT
ENV NICK=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV SERVER=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 22:54:57 GMT
ENV OWNER=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 22:54:57 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 22:54:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 22:54:57 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 22:54:57 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 22:54:58 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 22:54:58 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 22:54:58 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099eb2c394b0d326d520fdcc5f18a8fc772045d738fe77a2f240efab118e0d9b`  
		Last Modified: Wed, 14 Jun 2023 22:55:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc96b3f897fdcd18e5cda5ebe64ec173bbfd8da96d5d790e9b0fd73cefc79d`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e509faecac222671b3dd4d55f72a002ca5a682a47d68f82faf0510bd4537e5`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 2.8 MB (2776563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778ae48ae48085b17498690a77e4e6048a2ccf947f9a36640cecba18111a1b55`  
		Last Modified: Wed, 14 Jun 2023 22:55:27 GMT  
		Size: 6.2 MB (6187134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351a0886d9b67a435b0ad05bc1102cca13f87d0b00c9acea9271dbde6f057284`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457742eaec2ef43d65da8e6c10a538032d2d076549399118c397804c11c2ed72`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.5`

```console
$ docker pull eggdrop@sha256:3d23b6c36a7a3c389ab7d65c8d9408083d7513e6e9d1e7eb9531001e4dfdd07a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9.5` - linux; amd64

```console
$ docker pull eggdrop@sha256:fbb76e4f3fd2ee92563febb33b858d7bfc23e8a4ae90e77a0e6f065d7cd63f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11727481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5a2e0d5610d91f6e6b5b086fbc0a0e1f8413c9c9c52d6b8b4818b903ea7b42`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:42:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 15 Jun 2023 04:42:23 GMT
RUN adduser -S eggdrop
# Thu, 15 Jun 2023 04:42:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 15 Jun 2023 04:42:25 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 15 Jun 2023 04:46:22 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 15 Jun 2023 04:46:22 GMT
ENV NICK=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV SERVER=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV LISTEN=3333
# Thu, 15 Jun 2023 04:46:23 GMT
ENV OWNER=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV USERFILE=eggdrop.user
# Thu, 15 Jun 2023 04:46:23 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 15 Jun 2023 04:46:23 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 15 Jun 2023 04:46:23 GMT
EXPOSE 3333
# Thu, 15 Jun 2023 04:46:23 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 15 Jun 2023 04:46:23 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 15 Jun 2023 04:46:23 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 15 Jun 2023 04:46:23 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d216fc621c25522e777539ef90b86c566f8e186359154b2bfab46d0c793b0c9b`  
		Last Modified: Thu, 15 Jun 2023 04:46:47 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a5e16c27c10687f1f1b429526c75e1707ab0ea50ce602df684dda6b331f42`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 10.9 KB (10941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dc4cfb0d27369f3d3e88018e01f830d17dbdebe4b91ab24ccdbd3d6ba9d66a`  
		Last Modified: Thu, 15 Jun 2023 04:46:46 GMT  
		Size: 2.8 MB (2758065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8419a4c44d78db125dcd808f917e289ee923e5ee4b68758d01a3504a4745766d`  
		Last Modified: Thu, 15 Jun 2023 04:46:46 GMT  
		Size: 6.1 MB (6146999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c25e7ab8efa8ccdd354e83f46706704a0198eba17ccbf4964a827e3c8e7ff8a`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ebad7fb733ee98c26ad75a26d0b1b1d36e178e165faf0ed6a5fc8be1aaed6c`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.5` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:b8f18f32c6f50d3d622b687a62a98063626c1ebaad90b88615b01cce14c94f6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11363954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1faba54e962f458cbc99783a3c0429a3bdf9b487dfd87861c7e32eaaf592ac`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:28 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
# Wed, 14 Jun 2023 18:49:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 19:50:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 19:50:57 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 19:51:00 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 19:51:03 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 14 Jun 2023 19:56:08 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 19:56:08 GMT
ENV NICK=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV SERVER=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 19:56:09 GMT
ENV OWNER=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 19:56:09 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 19:56:09 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 19:56:09 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 19:56:09 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 19:56:09 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 19:56:09 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 19:56:09 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59edb5f625f9baba9a7ea41967538ecb65f8f3a2c21dbaac52c1cebdda71f4c5`  
		Last Modified: Wed, 14 Jun 2023 19:56:37 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d91c589e5b4c6197aed20876f69cbd4e6c2b756d05e459b7ac6bbcabe136c7`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 10.6 KB (10631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fdffc7323d45dd58aa0359aab7e2d9f9f375fddb9958fcd64fd770c94daf83`  
		Last Modified: Wed, 14 Jun 2023 19:56:36 GMT  
		Size: 2.7 MB (2679963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d7b4abdc31f67a9db93623090b78267d3fea57aef5ce525ffa72866261ccd`  
		Last Modified: Wed, 14 Jun 2023 19:56:37 GMT  
		Size: 6.1 MB (6053977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114272a2dc638a3349674767d3512c750bc67c2aa58ab072006c0c343c129aa8`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4afb0fc779b33a25070697e8911beeae28c81d7400a42941eee76a2e95ba1`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.5` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:30e1a07d96fd6931347842b9e336e3406c69a22af5a30ee3a6c6eede82c759db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11686144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95261f7f791cadf51418239f765292865cfdb39a9c8ac55c55c2addba62a289f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:51:05 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 22:51:05 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 22:51:06 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 22:51:08 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 14 Jun 2023 22:54:57 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 22:54:57 GMT
ENV NICK=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV SERVER=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 22:54:57 GMT
ENV OWNER=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 22:54:57 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 22:54:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 22:54:57 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 22:54:57 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 22:54:58 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 22:54:58 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 22:54:58 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099eb2c394b0d326d520fdcc5f18a8fc772045d738fe77a2f240efab118e0d9b`  
		Last Modified: Wed, 14 Jun 2023 22:55:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc96b3f897fdcd18e5cda5ebe64ec173bbfd8da96d5d790e9b0fd73cefc79d`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e509faecac222671b3dd4d55f72a002ca5a682a47d68f82faf0510bd4537e5`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 2.8 MB (2776563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778ae48ae48085b17498690a77e4e6048a2ccf947f9a36640cecba18111a1b55`  
		Last Modified: Wed, 14 Jun 2023 22:55:27 GMT  
		Size: 6.2 MB (6187134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351a0886d9b67a435b0ad05bc1102cca13f87d0b00c9acea9271dbde6f057284`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457742eaec2ef43d65da8e6c10a538032d2d076549399118c397804c11c2ed72`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:ad8499cf0120784c4a57db2b003e8c0cd71db3a8e2b16f799c3abb7f44cb7045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:beb13e638658e3b00b22b8d49f0f694ce40372c332caacd0b4fb899805e2f6b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16127511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:403fd9a31d4e69ba0897411e2818757e18a40f6645270de9d08560940d87a930`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:38:29 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 15 Jun 2023 04:38:29 GMT
RUN adduser -S eggdrop
# Thu, 15 Jun 2023 04:38:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 15 Jun 2023 04:38:30 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Thu, 15 Jun 2023 04:38:31 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Thu, 15 Jun 2023 04:38:32 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 15 Jun 2023 04:42:12 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 15 Jun 2023 04:42:12 GMT
ENV NICK=
# Thu, 15 Jun 2023 04:42:13 GMT
ENV SERVER=
# Thu, 15 Jun 2023 04:42:13 GMT
ENV LISTEN=3333
# Thu, 15 Jun 2023 04:42:13 GMT
ENV OWNER=
# Thu, 15 Jun 2023 04:42:13 GMT
ENV USERFILE=eggdrop.user
# Thu, 15 Jun 2023 04:42:13 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 15 Jun 2023 04:42:13 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 15 Jun 2023 04:42:13 GMT
EXPOSE 3333
# Thu, 15 Jun 2023 04:42:13 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Thu, 15 Jun 2023 04:42:13 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 15 Jun 2023 04:42:13 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 15 Jun 2023 04:42:13 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714c670ef22550a4a3ad9dd2eb8e0a56039cbdfb6748dc13d83eb3b347d0d5bd`  
		Last Modified: Thu, 15 Jun 2023 04:46:40 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc28894795b7ded44f6fc10e49e88ed71e71a3de7cda2b74c9818668bde3d03`  
		Last Modified: Thu, 15 Jun 2023 04:46:38 GMT  
		Size: 11.0 KB (10987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de551f5b9224829504860f0ebd32c88971602800fc8ff16e3ef56e552269cc80`  
		Last Modified: Thu, 15 Jun 2023 04:46:38 GMT  
		Size: 1.2 MB (1203427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead754afd421d8b5d6ad963afbbd03640b17040e38b7fcc20fbb779065c7cad0`  
		Last Modified: Thu, 15 Jun 2023 04:46:40 GMT  
		Size: 11.5 MB (11534163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ab9123a62b7db38c6d20c95a5fc287239ae4a695511c89fcbbe1c4e9db34f2`  
		Last Modified: Thu, 15 Jun 2023 04:46:38 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2687eb09fc414be6f8254fa2597136a4c68d65d0f62b6a8f57ed59f74bd4f9b`  
		Last Modified: Thu, 15 Jun 2023 04:46:38 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:b04c9ee90ae434c47a92e072bbe5b57531dbaa037afceaf1c681c13004a76b42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15727050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c20287fe40eb276e9686ef4bea510b90ebafc1975f35e844d5f9022befbd0b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 19:46:33 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 19:46:34 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 19:46:36 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 19:46:36 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Wed, 14 Jun 2023 19:46:37 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Wed, 14 Jun 2023 19:46:38 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 14 Jun 2023 19:50:44 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 19:50:44 GMT
ENV NICK=
# Wed, 14 Jun 2023 19:50:45 GMT
ENV SERVER=
# Wed, 14 Jun 2023 19:50:45 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 19:50:45 GMT
ENV OWNER=
# Wed, 14 Jun 2023 19:50:45 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 19:50:45 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 19:50:45 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 19:50:45 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 19:50:45 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 19:50:45 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 19:50:45 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 19:50:45 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da662cf081eacecc880868556d58fefa681f5a85748f715fa018059fc3610b9`  
		Last Modified: Wed, 14 Jun 2023 19:56:28 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1adc81653025f97685e7c96ba9145ecf37d5eb688af5653e202542ce7aa0af4`  
		Last Modified: Wed, 14 Jun 2023 19:56:26 GMT  
		Size: 11.1 KB (11135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b4e51f49c1a11557946eba1189df73b55efac200f2f9fdfcf88c4a2ccc789`  
		Last Modified: Wed, 14 Jun 2023 19:56:27 GMT  
		Size: 1.2 MB (1187432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b510499214f86b56fc84b2e8fce2d41a3c2ac6a01d3a339c5b6502e92f3968e8`  
		Last Modified: Wed, 14 Jun 2023 19:56:29 GMT  
		Size: 11.4 MB (11413335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6856ec7405ef9cab9d83cb843abb5b9880819c47362f0abd65c2adb821c61d33`  
		Last Modified: Wed, 14 Jun 2023 19:56:26 GMT  
		Size: 1.9 KB (1896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6058d001e9e054632a5c35775eaef1dc3e93a2b93e697f7d21e2d49ff024f6d0`  
		Last Modified: Wed, 14 Jun 2023 19:56:26 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:d6ee40eddcd6b4a135621b7b30c03b37126ea9caa8a0351ddabc3d3355e48154
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16104053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100ca47c5d29b68946c3c6b138af46476c2bb77c08d9c9829d9b71642a7cda37`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:47:42 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 22:47:42 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 22:47:44 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 22:47:44 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Wed, 14 Jun 2023 22:47:44 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Wed, 14 Jun 2023 22:47:45 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 14 Jun 2023 22:51:02 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 22:51:02 GMT
ENV NICK=
# Wed, 14 Jun 2023 22:51:02 GMT
ENV SERVER=
# Wed, 14 Jun 2023 22:51:02 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 22:51:02 GMT
ENV OWNER=
# Wed, 14 Jun 2023 22:51:02 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 22:51:02 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 22:51:02 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 22:51:03 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 22:51:03 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 22:51:03 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 22:51:03 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 22:51:03 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab556bb27c3eeadbcc437904e4d024f7ab53548eb269e2f05babbd5d673b7f06`  
		Last Modified: Wed, 14 Jun 2023 22:55:21 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821fe5f3cdc578d1e7bf2c18f3185bd991b368062f1a7c6b6edf42d1d1bd2c9c`  
		Last Modified: Wed, 14 Jun 2023 22:55:19 GMT  
		Size: 11.2 KB (11189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c154146375088dd23f935a6db1f78af30a7913b4a60903db68641c8822f425bc`  
		Last Modified: Wed, 14 Jun 2023 22:55:19 GMT  
		Size: 1.2 MB (1234460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b9bf5d321b4c83ed35be7d9f12decc16635c4dd88fb9aa9a6192ac3b26b237`  
		Last Modified: Wed, 14 Jun 2023 22:55:20 GMT  
		Size: 11.6 MB (11593040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821f8b68fcae9339ef33904560aade133f4b38dae0fa947938aa1b094651f365`  
		Last Modified: Wed, 14 Jun 2023 22:55:19 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae53839769fce95bc4bcf305e8d8bbf34e1820445b05c558cc53dd2dafd53aff`  
		Last Modified: Wed, 14 Jun 2023 22:55:19 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:3d23b6c36a7a3c389ab7d65c8d9408083d7513e6e9d1e7eb9531001e4dfdd07a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:fbb76e4f3fd2ee92563febb33b858d7bfc23e8a4ae90e77a0e6f065d7cd63f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11727481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5a2e0d5610d91f6e6b5b086fbc0a0e1f8413c9c9c52d6b8b4818b903ea7b42`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:42:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 15 Jun 2023 04:42:23 GMT
RUN adduser -S eggdrop
# Thu, 15 Jun 2023 04:42:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 15 Jun 2023 04:42:25 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 15 Jun 2023 04:46:22 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 15 Jun 2023 04:46:22 GMT
ENV NICK=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV SERVER=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV LISTEN=3333
# Thu, 15 Jun 2023 04:46:23 GMT
ENV OWNER=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV USERFILE=eggdrop.user
# Thu, 15 Jun 2023 04:46:23 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 15 Jun 2023 04:46:23 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 15 Jun 2023 04:46:23 GMT
EXPOSE 3333
# Thu, 15 Jun 2023 04:46:23 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 15 Jun 2023 04:46:23 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 15 Jun 2023 04:46:23 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 15 Jun 2023 04:46:23 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d216fc621c25522e777539ef90b86c566f8e186359154b2bfab46d0c793b0c9b`  
		Last Modified: Thu, 15 Jun 2023 04:46:47 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a5e16c27c10687f1f1b429526c75e1707ab0ea50ce602df684dda6b331f42`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 10.9 KB (10941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dc4cfb0d27369f3d3e88018e01f830d17dbdebe4b91ab24ccdbd3d6ba9d66a`  
		Last Modified: Thu, 15 Jun 2023 04:46:46 GMT  
		Size: 2.8 MB (2758065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8419a4c44d78db125dcd808f917e289ee923e5ee4b68758d01a3504a4745766d`  
		Last Modified: Thu, 15 Jun 2023 04:46:46 GMT  
		Size: 6.1 MB (6146999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c25e7ab8efa8ccdd354e83f46706704a0198eba17ccbf4964a827e3c8e7ff8a`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ebad7fb733ee98c26ad75a26d0b1b1d36e178e165faf0ed6a5fc8be1aaed6c`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:b8f18f32c6f50d3d622b687a62a98063626c1ebaad90b88615b01cce14c94f6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11363954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1faba54e962f458cbc99783a3c0429a3bdf9b487dfd87861c7e32eaaf592ac`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:28 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
# Wed, 14 Jun 2023 18:49:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 19:50:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 19:50:57 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 19:51:00 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 19:51:03 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 14 Jun 2023 19:56:08 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 19:56:08 GMT
ENV NICK=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV SERVER=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 19:56:09 GMT
ENV OWNER=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 19:56:09 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 19:56:09 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 19:56:09 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 19:56:09 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 19:56:09 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 19:56:09 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 19:56:09 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59edb5f625f9baba9a7ea41967538ecb65f8f3a2c21dbaac52c1cebdda71f4c5`  
		Last Modified: Wed, 14 Jun 2023 19:56:37 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d91c589e5b4c6197aed20876f69cbd4e6c2b756d05e459b7ac6bbcabe136c7`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 10.6 KB (10631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fdffc7323d45dd58aa0359aab7e2d9f9f375fddb9958fcd64fd770c94daf83`  
		Last Modified: Wed, 14 Jun 2023 19:56:36 GMT  
		Size: 2.7 MB (2679963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d7b4abdc31f67a9db93623090b78267d3fea57aef5ce525ffa72866261ccd`  
		Last Modified: Wed, 14 Jun 2023 19:56:37 GMT  
		Size: 6.1 MB (6053977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114272a2dc638a3349674767d3512c750bc67c2aa58ab072006c0c343c129aa8`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4afb0fc779b33a25070697e8911beeae28c81d7400a42941eee76a2e95ba1`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:30e1a07d96fd6931347842b9e336e3406c69a22af5a30ee3a6c6eede82c759db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11686144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95261f7f791cadf51418239f765292865cfdb39a9c8ac55c55c2addba62a289f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:51:05 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 22:51:05 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 22:51:06 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 22:51:08 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 14 Jun 2023 22:54:57 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 22:54:57 GMT
ENV NICK=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV SERVER=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 22:54:57 GMT
ENV OWNER=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 22:54:57 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 22:54:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 22:54:57 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 22:54:57 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 22:54:58 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 22:54:58 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 22:54:58 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099eb2c394b0d326d520fdcc5f18a8fc772045d738fe77a2f240efab118e0d9b`  
		Last Modified: Wed, 14 Jun 2023 22:55:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc96b3f897fdcd18e5cda5ebe64ec173bbfd8da96d5d790e9b0fd73cefc79d`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e509faecac222671b3dd4d55f72a002ca5a682a47d68f82faf0510bd4537e5`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 2.8 MB (2776563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778ae48ae48085b17498690a77e4e6048a2ccf947f9a36640cecba18111a1b55`  
		Last Modified: Wed, 14 Jun 2023 22:55:27 GMT  
		Size: 6.2 MB (6187134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351a0886d9b67a435b0ad05bc1102cca13f87d0b00c9acea9271dbde6f057284`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457742eaec2ef43d65da8e6c10a538032d2d076549399118c397804c11c2ed72`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:3d23b6c36a7a3c389ab7d65c8d9408083d7513e6e9d1e7eb9531001e4dfdd07a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:fbb76e4f3fd2ee92563febb33b858d7bfc23e8a4ae90e77a0e6f065d7cd63f20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11727481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5a2e0d5610d91f6e6b5b086fbc0a0e1f8413c9c9c52d6b8b4818b903ea7b42`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:42:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 15 Jun 2023 04:42:23 GMT
RUN adduser -S eggdrop
# Thu, 15 Jun 2023 04:42:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 15 Jun 2023 04:42:25 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 15 Jun 2023 04:46:22 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 15 Jun 2023 04:46:22 GMT
ENV NICK=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV SERVER=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV LISTEN=3333
# Thu, 15 Jun 2023 04:46:23 GMT
ENV OWNER=
# Thu, 15 Jun 2023 04:46:23 GMT
ENV USERFILE=eggdrop.user
# Thu, 15 Jun 2023 04:46:23 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 15 Jun 2023 04:46:23 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 15 Jun 2023 04:46:23 GMT
EXPOSE 3333
# Thu, 15 Jun 2023 04:46:23 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 15 Jun 2023 04:46:23 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 15 Jun 2023 04:46:23 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 15 Jun 2023 04:46:23 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d216fc621c25522e777539ef90b86c566f8e186359154b2bfab46d0c793b0c9b`  
		Last Modified: Thu, 15 Jun 2023 04:46:47 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a5e16c27c10687f1f1b429526c75e1707ab0ea50ce602df684dda6b331f42`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 10.9 KB (10941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dc4cfb0d27369f3d3e88018e01f830d17dbdebe4b91ab24ccdbd3d6ba9d66a`  
		Last Modified: Thu, 15 Jun 2023 04:46:46 GMT  
		Size: 2.8 MB (2758065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8419a4c44d78db125dcd808f917e289ee923e5ee4b68758d01a3504a4745766d`  
		Last Modified: Thu, 15 Jun 2023 04:46:46 GMT  
		Size: 6.1 MB (6146999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c25e7ab8efa8ccdd354e83f46706704a0198eba17ccbf4964a827e3c8e7ff8a`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ebad7fb733ee98c26ad75a26d0b1b1d36e178e165faf0ed6a5fc8be1aaed6c`  
		Last Modified: Thu, 15 Jun 2023 04:46:45 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:b8f18f32c6f50d3d622b687a62a98063626c1ebaad90b88615b01cce14c94f6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11363954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e1faba54e962f458cbc99783a3c0429a3bdf9b487dfd87861c7e32eaaf592ac`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:28 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
# Wed, 14 Jun 2023 18:49:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 19:50:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 19:50:57 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 19:51:00 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 19:51:03 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 14 Jun 2023 19:56:08 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 19:56:08 GMT
ENV NICK=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV SERVER=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 19:56:09 GMT
ENV OWNER=
# Wed, 14 Jun 2023 19:56:09 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 19:56:09 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 19:56:09 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 19:56:09 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 19:56:09 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 19:56:09 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 19:56:09 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 19:56:09 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59edb5f625f9baba9a7ea41967538ecb65f8f3a2c21dbaac52c1cebdda71f4c5`  
		Last Modified: Wed, 14 Jun 2023 19:56:37 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d91c589e5b4c6197aed20876f69cbd4e6c2b756d05e459b7ac6bbcabe136c7`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 10.6 KB (10631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fdffc7323d45dd58aa0359aab7e2d9f9f375fddb9958fcd64fd770c94daf83`  
		Last Modified: Wed, 14 Jun 2023 19:56:36 GMT  
		Size: 2.7 MB (2679963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d7b4abdc31f67a9db93623090b78267d3fea57aef5ce525ffa72866261ccd`  
		Last Modified: Wed, 14 Jun 2023 19:56:37 GMT  
		Size: 6.1 MB (6053977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114272a2dc638a3349674767d3512c750bc67c2aa58ab072006c0c343c129aa8`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4afb0fc779b33a25070697e8911beeae28c81d7400a42941eee76a2e95ba1`  
		Last Modified: Wed, 14 Jun 2023 19:56:35 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:30e1a07d96fd6931347842b9e336e3406c69a22af5a30ee3a6c6eede82c759db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11686144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95261f7f791cadf51418239f765292865cfdb39a9c8ac55c55c2addba62a289f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:51:05 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 22:51:05 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 22:51:06 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 22:51:08 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 14 Jun 2023 22:54:57 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 22:54:57 GMT
ENV NICK=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV SERVER=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 22:54:57 GMT
ENV OWNER=
# Wed, 14 Jun 2023 22:54:57 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 22:54:57 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 22:54:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 22:54:57 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 22:54:57 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 22:54:58 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 22:54:58 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 22:54:58 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099eb2c394b0d326d520fdcc5f18a8fc772045d738fe77a2f240efab118e0d9b`  
		Last Modified: Wed, 14 Jun 2023 22:55:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc96b3f897fdcd18e5cda5ebe64ec173bbfd8da96d5d790e9b0fd73cefc79d`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e509faecac222671b3dd4d55f72a002ca5a682a47d68f82faf0510bd4537e5`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 2.8 MB (2776563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778ae48ae48085b17498690a77e4e6048a2ccf947f9a36640cecba18111a1b55`  
		Last Modified: Wed, 14 Jun 2023 22:55:27 GMT  
		Size: 6.2 MB (6187134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351a0886d9b67a435b0ad05bc1102cca13f87d0b00c9acea9271dbde6f057284`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457742eaec2ef43d65da8e6c10a538032d2d076549399118c397804c11c2ed72`  
		Last Modified: Wed, 14 Jun 2023 22:55:26 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
