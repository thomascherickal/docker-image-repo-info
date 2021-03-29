<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.8`](#eggdrop18)
-	[`eggdrop:1.8.4`](#eggdrop184)
-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.0`](#eggdrop190)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.8`

```console
$ docker pull eggdrop@sha256:4ebea9e4a541f13bd1545c3af1a9718872c7468e24486c66d8c6a16fccbadbc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:1.8` - linux; amd64

```console
$ docker pull eggdrop@sha256:34144d980bb6efc6e4c058df849e6d100854c8ba9349f9351127a6de1688e790
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef158250e7fb9994b7f30c4a3ebd5241680ab83ce0165849e79192022682e2a5`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:56:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 26 Mar 2021 02:56:55 GMT
RUN adduser -S eggdrop
# Fri, 26 Mar 2021 02:56:56 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 26 Mar 2021 02:58:08 GMT
RUN apk add --no-cache tcl bash openssl
# Fri, 26 Mar 2021 02:59:04 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 26 Mar 2021 02:59:04 GMT
ENV NICK=
# Fri, 26 Mar 2021 02:59:04 GMT
ENV SERVER=
# Fri, 26 Mar 2021 02:59:04 GMT
ENV LISTEN=3333
# Fri, 26 Mar 2021 02:59:05 GMT
ENV OWNER=
# Fri, 26 Mar 2021 02:59:05 GMT
ENV USERFILE=eggdrop.user
# Fri, 26 Mar 2021 02:59:05 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 26 Mar 2021 02:59:05 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 26 Mar 2021 02:59:05 GMT
EXPOSE 3333
# Fri, 26 Mar 2021 02:59:06 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Fri, 26 Mar 2021 02:59:06 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 26 Mar 2021 02:59:06 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 26 Mar 2021 02:59:06 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142b4d4bcce7665a93979e1fe1f1091a8834f5695ba6201d0c301b29be4441e4`  
		Last Modified: Fri, 26 Mar 2021 02:59:30 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469ffc84df54c5381e18d169f6e0df862c133266f5b281787b3246642568fc70`  
		Last Modified: Fri, 26 Mar 2021 02:59:27 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34740657fbdbfb582c345ae6919a75dab157582f4f9d3dba664a89f2278131`  
		Last Modified: Fri, 26 Mar 2021 02:59:39 GMT  
		Size: 2.7 MB (2685262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe2f0f0cd37aa6c8c691e33d0093de598c1dc63a614b7299d11eed6d46d2261`  
		Last Modified: Fri, 26 Mar 2021 02:59:38 GMT  
		Size: 3.3 MB (3285740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58eaed9c609cfa2bc0235afe328efa191ac5b88d66d38905003c9ce0dcfef33`  
		Last Modified: Fri, 26 Mar 2021 02:59:38 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09b64b674578ef7bed9ca70980b1817371cfed3f2b4060455bc8d02f58a482`  
		Last Modified: Fri, 26 Mar 2021 02:59:38 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.8.4`

```console
$ docker pull eggdrop@sha256:4ebea9e4a541f13bd1545c3af1a9718872c7468e24486c66d8c6a16fccbadbc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:1.8.4` - linux; amd64

```console
$ docker pull eggdrop@sha256:34144d980bb6efc6e4c058df849e6d100854c8ba9349f9351127a6de1688e790
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef158250e7fb9994b7f30c4a3ebd5241680ab83ce0165849e79192022682e2a5`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:56:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 26 Mar 2021 02:56:55 GMT
RUN adduser -S eggdrop
# Fri, 26 Mar 2021 02:56:56 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 26 Mar 2021 02:58:08 GMT
RUN apk add --no-cache tcl bash openssl
# Fri, 26 Mar 2021 02:59:04 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 26 Mar 2021 02:59:04 GMT
ENV NICK=
# Fri, 26 Mar 2021 02:59:04 GMT
ENV SERVER=
# Fri, 26 Mar 2021 02:59:04 GMT
ENV LISTEN=3333
# Fri, 26 Mar 2021 02:59:05 GMT
ENV OWNER=
# Fri, 26 Mar 2021 02:59:05 GMT
ENV USERFILE=eggdrop.user
# Fri, 26 Mar 2021 02:59:05 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 26 Mar 2021 02:59:05 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 26 Mar 2021 02:59:05 GMT
EXPOSE 3333
# Fri, 26 Mar 2021 02:59:06 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Fri, 26 Mar 2021 02:59:06 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 26 Mar 2021 02:59:06 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 26 Mar 2021 02:59:06 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142b4d4bcce7665a93979e1fe1f1091a8834f5695ba6201d0c301b29be4441e4`  
		Last Modified: Fri, 26 Mar 2021 02:59:30 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469ffc84df54c5381e18d169f6e0df862c133266f5b281787b3246642568fc70`  
		Last Modified: Fri, 26 Mar 2021 02:59:27 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34740657fbdbfb582c345ae6919a75dab157582f4f9d3dba664a89f2278131`  
		Last Modified: Fri, 26 Mar 2021 02:59:39 GMT  
		Size: 2.7 MB (2685262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe2f0f0cd37aa6c8c691e33d0093de598c1dc63a614b7299d11eed6d46d2261`  
		Last Modified: Fri, 26 Mar 2021 02:59:38 GMT  
		Size: 3.3 MB (3285740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58eaed9c609cfa2bc0235afe328efa191ac5b88d66d38905003c9ce0dcfef33`  
		Last Modified: Fri, 26 Mar 2021 02:59:38 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09b64b674578ef7bed9ca70980b1817371cfed3f2b4060455bc8d02f58a482`  
		Last Modified: Fri, 26 Mar 2021 02:59:38 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:53c8ef3c6dbb2599a854aa4836b127b492076cf8043fe563745a72dd24b579c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:13010b6a4f764c6e5425d27686195f872847ec5921a7db5a8bfc4b41168c852b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8223857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e1b66b36045836215599980d50ddb3fd2bb467e8c4f7d66f0d70e4d82b2168`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:25:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:25:38 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:25:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:25:41 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:26:46 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:26:46 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:26:46 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:26:47 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:26:47 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:26:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:26:47 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:26:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:26:48 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:26:48 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:26:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99eb87d40a5d04bb2f3cddc6c0113a1f4a738519880cff4f1e07f650afc6dbf3`  
		Last Modified: Mon, 29 Mar 2021 18:27:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0b1ed597373f415721344f92df02c7699e1e113ec744bacb5ddfe5bd3173d9`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 10.1 KB (10109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e835b8b19e774c697d1793e108cd750e6c1892afb1297e469ba25dc9d2ba12`  
		Last Modified: Mon, 29 Mar 2021 18:27:29 GMT  
		Size: 2.7 MB (2724405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f89e026f3f26d697df684d26a88f117e9883d99d06ebeba67c6e6cfafa9e19`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 2.7 MB (2673861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da9cf0048a0a220ae0bf1a6d07c39a67c3a4c8d8799d669b4388228680e393f`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024f150310092d715076476be109a494ac27069acdddd796376344da55c6d533`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:a903b3eb088fbab72e75fdbffc3792cd7311ac445dcd0bf3e914c5bf9c58e564
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7921335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edd80bd286beab17a4624b8e275484d63f2c81eace241327185faf2a81b9e8c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:53:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:53:58 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:54:02 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:54:07 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:56:09 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:56:10 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:56:12 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:56:13 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:56:14 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:56:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:56:15 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:56:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:56:17 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:56:18 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:56:18 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d5795228fdf51c0b33e4b1030c55662bc5f4c74e902f62b13d97fd75eed011`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7255637a93148079c117c136fbe895bd9664e14272e77150a651f0a20c1f0e46`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 9.8 KB (9831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaaae1f2c8d48c68fb8b68fb32deedb84bf83aa061a17bbc6743f44168ef65c`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 2.7 MB (2652107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2016760df48209206db193fdf1b1870926d1e141260b961737e60d8887251c33`  
		Last Modified: Mon, 29 Mar 2021 18:56:47 GMT  
		Size: 2.6 MB (2633533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecff28645f9741a60c783a5dae112e9afc007731f566e1f677355b27ef27d57`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aadba0251233b4de0d549ff16b315ec5303a767277f1b49f18f35eec7083ac`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:aa869560547dc520f7327b8123c108ec394137a93befa2ec96742f6c3f4e7cec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8146606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d0f5e17e38fc11cecbc4aae1054fca1d1b46831a637640bced609cd9e10661`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:41:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:41:59 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:42:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:42:08 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:44:06 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:44:07 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:44:08 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:44:09 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:44:10 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:44:10 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:44:11 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:44:12 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:44:13 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:44:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:44:15 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:44:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:44:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7908687cab4e2e8036d3a15a7b35c59c0fb94a48df7adc80fecbf7f62b1e37f`  
		Last Modified: Mon, 29 Mar 2021 18:44:43 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed4b45bb3f885133e6216b64ea7b52fd184ceaff01b3f065710c2d4a5a75e6f`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 10.0 KB (9994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5efde971466056a68596f83fa25c975d505e70d57c8ab24c47c16808aaeed4`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.8 MB (2752513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d1479a7f297db755dad66c514bc3a85053294cb58f8ae47793a7efaf496b9e`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.7 MB (2668400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808a387447375f7ffae93dc4ee79e97f9fede109c952002b5b01d1b79b7abc1e`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eeef541bea0e9378eff40154ba040f95a9ac50d2c4b7f4e2b0ced63f3e1b1c`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.0`

```console
$ docker pull eggdrop@sha256:53c8ef3c6dbb2599a854aa4836b127b492076cf8043fe563745a72dd24b579c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9.0` - linux; amd64

```console
$ docker pull eggdrop@sha256:13010b6a4f764c6e5425d27686195f872847ec5921a7db5a8bfc4b41168c852b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8223857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e1b66b36045836215599980d50ddb3fd2bb467e8c4f7d66f0d70e4d82b2168`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:25:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:25:38 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:25:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:25:41 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:26:46 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:26:46 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:26:46 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:26:47 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:26:47 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:26:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:26:47 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:26:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:26:48 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:26:48 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:26:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99eb87d40a5d04bb2f3cddc6c0113a1f4a738519880cff4f1e07f650afc6dbf3`  
		Last Modified: Mon, 29 Mar 2021 18:27:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0b1ed597373f415721344f92df02c7699e1e113ec744bacb5ddfe5bd3173d9`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 10.1 KB (10109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e835b8b19e774c697d1793e108cd750e6c1892afb1297e469ba25dc9d2ba12`  
		Last Modified: Mon, 29 Mar 2021 18:27:29 GMT  
		Size: 2.7 MB (2724405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f89e026f3f26d697df684d26a88f117e9883d99d06ebeba67c6e6cfafa9e19`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 2.7 MB (2673861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da9cf0048a0a220ae0bf1a6d07c39a67c3a4c8d8799d669b4388228680e393f`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024f150310092d715076476be109a494ac27069acdddd796376344da55c6d533`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.0` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:a903b3eb088fbab72e75fdbffc3792cd7311ac445dcd0bf3e914c5bf9c58e564
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7921335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edd80bd286beab17a4624b8e275484d63f2c81eace241327185faf2a81b9e8c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:53:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:53:58 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:54:02 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:54:07 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:56:09 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:56:10 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:56:12 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:56:13 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:56:14 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:56:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:56:15 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:56:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:56:17 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:56:18 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:56:18 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d5795228fdf51c0b33e4b1030c55662bc5f4c74e902f62b13d97fd75eed011`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7255637a93148079c117c136fbe895bd9664e14272e77150a651f0a20c1f0e46`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 9.8 KB (9831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaaae1f2c8d48c68fb8b68fb32deedb84bf83aa061a17bbc6743f44168ef65c`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 2.7 MB (2652107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2016760df48209206db193fdf1b1870926d1e141260b961737e60d8887251c33`  
		Last Modified: Mon, 29 Mar 2021 18:56:47 GMT  
		Size: 2.6 MB (2633533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecff28645f9741a60c783a5dae112e9afc007731f566e1f677355b27ef27d57`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aadba0251233b4de0d549ff16b315ec5303a767277f1b49f18f35eec7083ac`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.0` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:aa869560547dc520f7327b8123c108ec394137a93befa2ec96742f6c3f4e7cec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8146606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d0f5e17e38fc11cecbc4aae1054fca1d1b46831a637640bced609cd9e10661`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:41:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:41:59 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:42:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:42:08 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:44:06 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:44:07 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:44:08 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:44:09 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:44:10 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:44:10 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:44:11 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:44:12 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:44:13 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:44:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:44:15 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:44:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:44:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7908687cab4e2e8036d3a15a7b35c59c0fb94a48df7adc80fecbf7f62b1e37f`  
		Last Modified: Mon, 29 Mar 2021 18:44:43 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed4b45bb3f885133e6216b64ea7b52fd184ceaff01b3f065710c2d4a5a75e6f`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 10.0 KB (9994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5efde971466056a68596f83fa25c975d505e70d57c8ab24c47c16808aaeed4`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.8 MB (2752513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d1479a7f297db755dad66c514bc3a85053294cb58f8ae47793a7efaf496b9e`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.7 MB (2668400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808a387447375f7ffae93dc4ee79e97f9fede109c952002b5b01d1b79b7abc1e`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eeef541bea0e9378eff40154ba040f95a9ac50d2c4b7f4e2b0ced63f3e1b1c`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:3560c6b621db21e28dcaf2c228228462647d517ae95c0baa82d47e7fc3c53a6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:8f95248afc41765a29beb58ccc1e0a9100d08d5ede19ef97409477791ca32612
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13902123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e552ecd7552a7847ed7b136a36966d161d21e02e5246469c1b4b890d74b82bc`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:56:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 26 Mar 2021 02:56:55 GMT
RUN adduser -S eggdrop
# Fri, 26 Mar 2021 02:56:56 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:24:34 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Mon, 29 Mar 2021 18:24:34 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Mon, 29 Mar 2021 18:24:36 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:25:28 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:25:28 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:25:28 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:25:28 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:25:29 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:25:29 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:25:29 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:25:29 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:25:29 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:25:30 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:25:30 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:25:30 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:25:30 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142b4d4bcce7665a93979e1fe1f1091a8834f5695ba6201d0c301b29be4441e4`  
		Last Modified: Fri, 26 Mar 2021 02:59:30 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469ffc84df54c5381e18d169f6e0df862c133266f5b281787b3246642568fc70`  
		Last Modified: Fri, 26 Mar 2021 02:59:27 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e57bf86a973cb83d31a427604abaccd148b7c853e5c6137ab144e3028213f9`  
		Last Modified: Mon, 29 Mar 2021 18:27:13 GMT  
		Size: 2.7 MB (2685239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be535f19a02b245ba61a262e0612ecc66548375af9b8454484537556810a03b`  
		Last Modified: Mon, 29 Mar 2021 18:27:17 GMT  
		Size: 8.4 MB (8388116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171725a54e3e8597c978a73daf2f84f2357054d3acd625b0d9d949d3ec800bbb`  
		Last Modified: Mon, 29 Mar 2021 18:27:12 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36fac86a2219703eededd0389b1d37904afb794fd8ae615606c08f5a811b7eb`  
		Last Modified: Mon, 29 Mar 2021 18:27:12 GMT  
		Size: 707.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:ce80af1cdfb584a75094f264d3d3a5f7c231308dc127c41d16733219e90f112e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d22d7040cd5b308e67200d0e50ef1ebd7050ca3b19e1daf5f0fe73e5b47da54`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:18:05 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 26 Mar 2021 00:18:08 GMT
RUN adduser -S eggdrop
# Fri, 26 Mar 2021 00:18:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:51:22 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Mon, 29 Mar 2021 18:51:23 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Mon, 29 Mar 2021 18:51:27 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:53:26 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:53:27 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:53:28 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:53:29 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:53:29 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:53:31 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:53:32 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:53:33 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:53:34 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:53:34 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:53:35 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:53:36 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:53:37 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34be1b52d02353764116f4b71c27c3531ae363dea14dd7f7ec291e807459551`  
		Last Modified: Fri, 26 Mar 2021 00:20:46 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df3fec63b7b30cda31cc85a0837f550ae13c58ce96c042da4c668890e54fc73`  
		Last Modified: Fri, 26 Mar 2021 00:20:44 GMT  
		Size: 9.4 KB (9396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f128b680f02dbe67ef96886c94570bfd2fc8344777a5a45bdc138316bfcabc`  
		Last Modified: Mon, 29 Mar 2021 18:56:40 GMT  
		Size: 2.6 MB (2608729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53788357bfe903c57109fb9a80851f2226f1313bd2a3e5fb39da8fbb01ddccf1`  
		Last Modified: Mon, 29 Mar 2021 18:56:42 GMT  
		Size: 8.3 MB (8316623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0fe9eb83df466d892892c8925e79f869731157cc5c8df28af4241d02120a21`  
		Last Modified: Mon, 29 Mar 2021 18:56:39 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8123a7a0447cb93522917f7fa914d8fdb6385d391ffccbb18ba3bd30260828dc`  
		Last Modified: Mon, 29 Mar 2021 18:56:39 GMT  
		Size: 709.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:ebe4c505999bac107006caab3087a19b1626660816a56fab4c779b4d75633749
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13868609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:175504aa01bd3ba6d34a5ed5002a36115f486789e6baf4ff32c6ca807ac190b4`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:57:18 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 25 Mar 2021 23:57:41 GMT
RUN adduser -S eggdrop
# Thu, 25 Mar 2021 23:58:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:39:36 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Mon, 29 Mar 2021 18:39:36 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Mon, 29 Mar 2021 18:39:41 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:41:31 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:41:32 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:41:33 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:41:34 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:41:35 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:41:36 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:41:38 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:41:39 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:41:40 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:41:41 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:41:42 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:41:43 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:41:44 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016b21c12c3099ed521797a14ada34ef399a4c317694fda20c5c7b800f40d8a6`  
		Last Modified: Fri, 26 Mar 2021 00:03:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c4ae16ae920d6a492c4d547d7a976f7560f0b85134e15660d9260ba12bf09`  
		Last Modified: Fri, 26 Mar 2021 00:03:30 GMT  
		Size: 9.5 KB (9514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65d34f70a023ecfd180699f8cc86239b7878512187ea08fe95b3251721bf1e`  
		Last Modified: Mon, 29 Mar 2021 18:44:34 GMT  
		Size: 2.7 MB (2722576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be134728433202b3225918a48165a44a5ef4b1a1c9da7f3d2e74fa50b01a8381`  
		Last Modified: Mon, 29 Mar 2021 18:44:35 GMT  
		Size: 8.4 MB (8406782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060a30b23d1fc14460b63cd1901c866929eca6588f4d8b95fb29f8749d68cdb`  
		Last Modified: Mon, 29 Mar 2021 18:44:33 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2371a756868028c8d516492b08889dad36efe78df674139a471d0fdb803279bb`  
		Last Modified: Mon, 29 Mar 2021 18:44:34 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:53c8ef3c6dbb2599a854aa4836b127b492076cf8043fe563745a72dd24b579c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:13010b6a4f764c6e5425d27686195f872847ec5921a7db5a8bfc4b41168c852b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8223857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e1b66b36045836215599980d50ddb3fd2bb467e8c4f7d66f0d70e4d82b2168`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:25:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:25:38 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:25:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:25:41 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:26:46 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:26:46 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:26:46 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:26:47 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:26:47 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:26:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:26:47 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:26:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:26:48 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:26:48 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:26:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99eb87d40a5d04bb2f3cddc6c0113a1f4a738519880cff4f1e07f650afc6dbf3`  
		Last Modified: Mon, 29 Mar 2021 18:27:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0b1ed597373f415721344f92df02c7699e1e113ec744bacb5ddfe5bd3173d9`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 10.1 KB (10109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e835b8b19e774c697d1793e108cd750e6c1892afb1297e469ba25dc9d2ba12`  
		Last Modified: Mon, 29 Mar 2021 18:27:29 GMT  
		Size: 2.7 MB (2724405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f89e026f3f26d697df684d26a88f117e9883d99d06ebeba67c6e6cfafa9e19`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 2.7 MB (2673861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da9cf0048a0a220ae0bf1a6d07c39a67c3a4c8d8799d669b4388228680e393f`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024f150310092d715076476be109a494ac27069acdddd796376344da55c6d533`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:a903b3eb088fbab72e75fdbffc3792cd7311ac445dcd0bf3e914c5bf9c58e564
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7921335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edd80bd286beab17a4624b8e275484d63f2c81eace241327185faf2a81b9e8c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:53:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:53:58 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:54:02 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:54:07 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:56:09 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:56:10 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:56:12 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:56:13 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:56:14 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:56:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:56:15 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:56:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:56:17 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:56:18 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:56:18 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d5795228fdf51c0b33e4b1030c55662bc5f4c74e902f62b13d97fd75eed011`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7255637a93148079c117c136fbe895bd9664e14272e77150a651f0a20c1f0e46`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 9.8 KB (9831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaaae1f2c8d48c68fb8b68fb32deedb84bf83aa061a17bbc6743f44168ef65c`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 2.7 MB (2652107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2016760df48209206db193fdf1b1870926d1e141260b961737e60d8887251c33`  
		Last Modified: Mon, 29 Mar 2021 18:56:47 GMT  
		Size: 2.6 MB (2633533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecff28645f9741a60c783a5dae112e9afc007731f566e1f677355b27ef27d57`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aadba0251233b4de0d549ff16b315ec5303a767277f1b49f18f35eec7083ac`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:aa869560547dc520f7327b8123c108ec394137a93befa2ec96742f6c3f4e7cec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8146606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d0f5e17e38fc11cecbc4aae1054fca1d1b46831a637640bced609cd9e10661`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:41:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:41:59 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:42:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:42:08 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:44:06 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:44:07 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:44:08 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:44:09 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:44:10 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:44:10 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:44:11 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:44:12 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:44:13 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:44:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:44:15 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:44:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:44:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7908687cab4e2e8036d3a15a7b35c59c0fb94a48df7adc80fecbf7f62b1e37f`  
		Last Modified: Mon, 29 Mar 2021 18:44:43 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed4b45bb3f885133e6216b64ea7b52fd184ceaff01b3f065710c2d4a5a75e6f`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 10.0 KB (9994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5efde971466056a68596f83fa25c975d505e70d57c8ab24c47c16808aaeed4`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.8 MB (2752513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d1479a7f297db755dad66c514bc3a85053294cb58f8ae47793a7efaf496b9e`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.7 MB (2668400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808a387447375f7ffae93dc4ee79e97f9fede109c952002b5b01d1b79b7abc1e`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eeef541bea0e9378eff40154ba040f95a9ac50d2c4b7f4e2b0ced63f3e1b1c`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:53c8ef3c6dbb2599a854aa4836b127b492076cf8043fe563745a72dd24b579c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:13010b6a4f764c6e5425d27686195f872847ec5921a7db5a8bfc4b41168c852b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8223857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e1b66b36045836215599980d50ddb3fd2bb467e8c4f7d66f0d70e4d82b2168`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:25:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:25:38 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:25:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:25:41 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:26:46 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:26:46 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:26:46 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:26:47 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:26:47 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:26:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:26:47 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:26:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:26:48 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:26:48 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:26:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99eb87d40a5d04bb2f3cddc6c0113a1f4a738519880cff4f1e07f650afc6dbf3`  
		Last Modified: Mon, 29 Mar 2021 18:27:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0b1ed597373f415721344f92df02c7699e1e113ec744bacb5ddfe5bd3173d9`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 10.1 KB (10109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e835b8b19e774c697d1793e108cd750e6c1892afb1297e469ba25dc9d2ba12`  
		Last Modified: Mon, 29 Mar 2021 18:27:29 GMT  
		Size: 2.7 MB (2724405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f89e026f3f26d697df684d26a88f117e9883d99d06ebeba67c6e6cfafa9e19`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 2.7 MB (2673861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da9cf0048a0a220ae0bf1a6d07c39a67c3a4c8d8799d669b4388228680e393f`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024f150310092d715076476be109a494ac27069acdddd796376344da55c6d533`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:a903b3eb088fbab72e75fdbffc3792cd7311ac445dcd0bf3e914c5bf9c58e564
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7921335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edd80bd286beab17a4624b8e275484d63f2c81eace241327185faf2a81b9e8c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:53:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:53:58 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:54:02 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:54:07 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:56:09 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:56:10 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:56:12 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:56:13 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:56:14 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:56:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:56:15 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:56:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:56:17 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:56:18 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:56:18 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d5795228fdf51c0b33e4b1030c55662bc5f4c74e902f62b13d97fd75eed011`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7255637a93148079c117c136fbe895bd9664e14272e77150a651f0a20c1f0e46`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 9.8 KB (9831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaaae1f2c8d48c68fb8b68fb32deedb84bf83aa061a17bbc6743f44168ef65c`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 2.7 MB (2652107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2016760df48209206db193fdf1b1870926d1e141260b961737e60d8887251c33`  
		Last Modified: Mon, 29 Mar 2021 18:56:47 GMT  
		Size: 2.6 MB (2633533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecff28645f9741a60c783a5dae112e9afc007731f566e1f677355b27ef27d57`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aadba0251233b4de0d549ff16b315ec5303a767277f1b49f18f35eec7083ac`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:aa869560547dc520f7327b8123c108ec394137a93befa2ec96742f6c3f4e7cec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8146606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d0f5e17e38fc11cecbc4aae1054fca1d1b46831a637640bced609cd9e10661`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:41:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:41:59 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:42:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:42:08 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:44:06 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:44:07 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:44:08 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:44:09 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:44:10 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:44:10 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:44:11 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:44:12 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:44:13 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:44:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:44:15 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:44:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:44:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7908687cab4e2e8036d3a15a7b35c59c0fb94a48df7adc80fecbf7f62b1e37f`  
		Last Modified: Mon, 29 Mar 2021 18:44:43 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed4b45bb3f885133e6216b64ea7b52fd184ceaff01b3f065710c2d4a5a75e6f`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 10.0 KB (9994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5efde971466056a68596f83fa25c975d505e70d57c8ab24c47c16808aaeed4`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.8 MB (2752513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d1479a7f297db755dad66c514bc3a85053294cb58f8ae47793a7efaf496b9e`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.7 MB (2668400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808a387447375f7ffae93dc4ee79e97f9fede109c952002b5b01d1b79b7abc1e`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eeef541bea0e9378eff40154ba040f95a9ac50d2c4b7f4e2b0ced63f3e1b1c`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
