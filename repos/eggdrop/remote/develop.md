## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:c6be7509b7fe340023350f20ea9156ab15b3187815be7d0404ca1258f90ff6f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:f2f7522c1d553396db47974bee3f18fcd91752de34d6470b33a49bd115e03496
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13235144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7370cd0da7a9c5fb8e8b479c6daf2941e51fcf0895b460d266218ef8818d828`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:23:46 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 24 Feb 2021 21:23:48 GMT
RUN adduser -S eggdrop
# Wed, 24 Feb 2021 21:23:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 24 Feb 2021 21:23:51 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Wed, 24 Feb 2021 21:23:51 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Wed, 24 Feb 2021 21:23:54 GMT
RUN apk --update add --no-cache tcl bash openssl
# Wed, 24 Feb 2021 21:24:55 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 24 Feb 2021 21:24:55 GMT
ENV NICK=
# Wed, 24 Feb 2021 21:24:56 GMT
ENV SERVER=
# Wed, 24 Feb 2021 21:24:56 GMT
ENV LISTEN=3333
# Wed, 24 Feb 2021 21:24:56 GMT
ENV OWNER=
# Wed, 24 Feb 2021 21:24:56 GMT
ENV USERFILE=eggdrop.user
# Wed, 24 Feb 2021 21:24:56 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 24 Feb 2021 21:24:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 24 Feb 2021 21:24:57 GMT
EXPOSE 3333
# Wed, 24 Feb 2021 21:24:57 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Wed, 24 Feb 2021 21:24:57 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 24 Feb 2021 21:24:57 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 24 Feb 2021 21:24:58 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a622212a04444901eef71ac1a5abe89e7eb5812de71c73fa5493573bf18b52`  
		Last Modified: Wed, 24 Feb 2021 21:26:27 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4a9cd3c9326ce9d816f5be5eb6f75f0a433941031aca2506e53c19765eee3`  
		Last Modified: Wed, 24 Feb 2021 21:26:26 GMT  
		Size: 9.6 KB (9577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a28507ba3b1d703893d38412247659ce1e0ca8e5f4c116ead57bcf21d164b3c`  
		Last Modified: Wed, 24 Feb 2021 21:26:27 GMT  
		Size: 2.7 MB (2684856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28de84a7fec123bb2c6268e723121b4958f04f51b3f082ac22d948ed68b0dc8e`  
		Last Modified: Wed, 24 Feb 2021 21:26:29 GMT  
		Size: 7.7 MB (7721581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b2287cc307a2059cf6bdd886bed89836406563fa30b0464ee23eacb315f058`  
		Last Modified: Wed, 24 Feb 2021 21:26:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa2ce0434175256b1d94a88cb0364bcbf937c783285bc88ad4a763440735201`  
		Last Modified: Wed, 24 Feb 2021 21:26:26 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:4b3094c40be6f330dbab4fbeda61553e4613d3c417f2b4a91cde133ef08fd041
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12901992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14d21d777b1e0d70bc5ae7bee67940ea691dfe2d63bd73472d8eebda2b2b5ff3`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:28:14 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 25 Feb 2021 00:28:19 GMT
RUN adduser -S eggdrop
# Thu, 25 Feb 2021 00:28:26 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 25 Feb 2021 00:28:27 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Thu, 25 Feb 2021 00:28:28 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Thu, 25 Feb 2021 00:28:36 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 25 Feb 2021 00:31:00 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 25 Feb 2021 00:31:01 GMT
ENV NICK=
# Thu, 25 Feb 2021 00:31:02 GMT
ENV SERVER=
# Thu, 25 Feb 2021 00:31:05 GMT
ENV LISTEN=3333
# Thu, 25 Feb 2021 00:31:06 GMT
ENV OWNER=
# Thu, 25 Feb 2021 00:31:06 GMT
ENV USERFILE=eggdrop.user
# Thu, 25 Feb 2021 00:31:08 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 25 Feb 2021 00:31:09 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 25 Feb 2021 00:31:09 GMT
EXPOSE 3333
# Thu, 25 Feb 2021 00:31:10 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 25 Feb 2021 00:31:11 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 25 Feb 2021 00:31:11 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 25 Feb 2021 00:31:12 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe21623383fe574b3935c80d4ce081e4d39972c5dc4ad9c8c4bf20e6217d48e`  
		Last Modified: Thu, 25 Feb 2021 00:31:24 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616eb1b2593f122b2ec5a336cdbcd5303f22e4f03d6ebf4330df96aa5f49bac7`  
		Last Modified: Thu, 25 Feb 2021 00:31:22 GMT  
		Size: 9.4 KB (9398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d7fb4c9403f7bba1475ecae68789770a3ccacc773bae5b817b32600036a459`  
		Last Modified: Thu, 25 Feb 2021 00:31:23 GMT  
		Size: 2.6 MB (2608767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193b154170e7a6fa01a551e40d88acc4e5d35b00e07e66ff7ca60078fc092938`  
		Last Modified: Thu, 25 Feb 2021 00:31:24 GMT  
		Size: 7.7 MB (7658916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f81bbfabcc7eaba6562679f08a333c3a644001b64446e3ebd8b567ea7941591`  
		Last Modified: Thu, 25 Feb 2021 00:31:22 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d616bd16ba3068f9bfd65523b6fe8a47518257c6bb6e1917d00476eb1d6732cb`  
		Last Modified: Thu, 25 Feb 2021 00:31:22 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:71f52c23af6f2daa089fc33af9d9536c5e59b08e52eda6e5dced04c81b492d14
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13196522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:092efcaec504a10ec4ddba863da45dd5e9ba858beb5b6a21e2f88319b9bab29b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:40:21 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 24 Feb 2021 21:40:23 GMT
RUN adduser -S eggdrop
# Wed, 24 Feb 2021 21:40:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 24 Feb 2021 21:40:26 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Wed, 24 Feb 2021 21:40:27 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Wed, 24 Feb 2021 21:40:30 GMT
RUN apk --update add --no-cache tcl bash openssl
# Wed, 24 Feb 2021 21:42:19 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 24 Feb 2021 21:42:20 GMT
ENV NICK=
# Wed, 24 Feb 2021 21:42:21 GMT
ENV SERVER=
# Wed, 24 Feb 2021 21:42:22 GMT
ENV LISTEN=3333
# Wed, 24 Feb 2021 21:42:23 GMT
ENV OWNER=
# Wed, 24 Feb 2021 21:42:24 GMT
ENV USERFILE=eggdrop.user
# Wed, 24 Feb 2021 21:42:24 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 24 Feb 2021 21:42:25 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 24 Feb 2021 21:42:27 GMT
EXPOSE 3333
# Wed, 24 Feb 2021 21:42:28 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Wed, 24 Feb 2021 21:42:28 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 24 Feb 2021 21:42:30 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 24 Feb 2021 21:42:30 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d7e620a18c70da62d98fd84649c1aa6e9bace50def7eb2c177a1e5bd7a5a88`  
		Last Modified: Wed, 24 Feb 2021 21:42:46 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473de84245e87f528cf9f16d91909982599e6ba23d12d914bf8aa0770f103bb4`  
		Last Modified: Wed, 24 Feb 2021 21:42:45 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1799fa8d5985e242d43d030c3e54d5b524b56936a35c3e6cb66da68717dc97ea`  
		Last Modified: Wed, 24 Feb 2021 21:42:45 GMT  
		Size: 2.7 MB (2722535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c2f7eac06eaf8d77aaa1777f7afeac03d07528ce38738b208c3f6ac16f12c`  
		Last Modified: Wed, 24 Feb 2021 21:42:46 GMT  
		Size: 7.7 MB (7734807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf252e5213cca7ba05fd7b5c490ff151967233b84462b389d30a49c6f64fd0e`  
		Last Modified: Wed, 24 Feb 2021 21:42:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8014ed58e96e64c1c174936c8de6d6409e392d5fa2920561f15a7050f274127b`  
		Last Modified: Wed, 24 Feb 2021 21:42:44 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
