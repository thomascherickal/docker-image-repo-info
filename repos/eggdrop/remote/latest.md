## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:146b83aee861ed19417e6fa50a927e90bf09a5aca228caa175997b8d919df634
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:eabffed140b80fa13a363774b61aa6e1f3fd8304c0f3563413e82050f953f6c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8224313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c447c0db30c0f6e883c7216be31dda5e32e2ea27b52a9b8f5c8011faa2aebb71`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:11:23 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 01 Apr 2021 14:11:24 GMT
RUN adduser -S eggdrop
# Thu, 01 Apr 2021 14:11:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 01 Apr 2021 14:11:27 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 01 Apr 2021 14:12:23 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 01 Apr 2021 14:12:23 GMT
ENV NICK=
# Thu, 01 Apr 2021 14:12:24 GMT
ENV SERVER=
# Thu, 01 Apr 2021 14:12:24 GMT
ENV LISTEN=3333
# Thu, 01 Apr 2021 14:12:24 GMT
ENV OWNER=
# Thu, 01 Apr 2021 14:12:24 GMT
ENV USERFILE=eggdrop.user
# Thu, 01 Apr 2021 14:12:24 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 01 Apr 2021 14:12:25 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 01 Apr 2021 14:12:25 GMT
EXPOSE 3333
# Thu, 01 Apr 2021 14:12:25 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 01 Apr 2021 14:12:25 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 01 Apr 2021 14:12:25 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 01 Apr 2021 14:12:26 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42095f7eac21c504e274fb4305d2590b148938f70eb1b6400a1523d06d5dbd0`  
		Last Modified: Thu, 01 Apr 2021 14:13:18 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f1d7098a41ec2df4414024aed354715c0252e87c9c54687c96bef9dc958885`  
		Last Modified: Thu, 01 Apr 2021 14:13:15 GMT  
		Size: 10.1 KB (10115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d88a8485b20770aa1decab4b1cba8746f54cfe4beb93dc0bfa505412e7be7a9`  
		Last Modified: Thu, 01 Apr 2021 14:13:16 GMT  
		Size: 2.7 MB (2724573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de035d9c1cb0e478beff649ecca8d9ddb1d543f6fe094b743fd48678cf3e8167`  
		Last Modified: Thu, 01 Apr 2021 14:13:16 GMT  
		Size: 2.7 MB (2673878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec84ade4cd51fe32e1cd3185531d6cd61fdc18dad25bc3bc520f4d3daf0bc52`  
		Last Modified: Thu, 01 Apr 2021 14:13:15 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc572fc82156d83568641971caa0529923fbc0aeac8b1c1f71bc72a96ea9aab`  
		Last Modified: Thu, 01 Apr 2021 14:13:15 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:aec1e8d64ab1e7287f6b9c1c7991a1562b4b794d77931d75542a5fda37471472
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7921383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc484287ff1b50155f08697db75e244702a5c27467145a8c40ca8002b485a0b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:29:11 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 31 Mar 2021 19:29:17 GMT
RUN adduser -S eggdrop
# Wed, 31 Mar 2021 19:29:23 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 31 Mar 2021 19:29:31 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 31 Mar 2021 19:32:12 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 31 Mar 2021 19:32:13 GMT
ENV NICK=
# Wed, 31 Mar 2021 19:32:15 GMT
ENV SERVER=
# Wed, 31 Mar 2021 19:32:15 GMT
ENV LISTEN=3333
# Wed, 31 Mar 2021 19:32:16 GMT
ENV OWNER=
# Wed, 31 Mar 2021 19:32:17 GMT
ENV USERFILE=eggdrop.user
# Wed, 31 Mar 2021 19:32:18 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 31 Mar 2021 19:32:19 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 31 Mar 2021 19:32:19 GMT
EXPOSE 3333
# Wed, 31 Mar 2021 19:32:20 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 31 Mar 2021 19:32:21 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 31 Mar 2021 19:32:22 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 31 Mar 2021 19:32:22 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8e825d0673b1409e4dbdb8d11420d3548926c7ec06471892c81459e7e0d09c`  
		Last Modified: Wed, 31 Mar 2021 19:33:03 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0da49ceef750484d93aa4007ce4f01a1666c837942ef9d945a16c9b2632dc8e`  
		Last Modified: Wed, 31 Mar 2021 19:33:01 GMT  
		Size: 9.8 KB (9827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134921cf54ec8713f3a15bc2d9394074aa568ae849eae467885486a2d67d0667`  
		Last Modified: Wed, 31 Mar 2021 19:33:04 GMT  
		Size: 2.7 MB (2652129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3215ac4092c427e26144436537fd2a9885bc701488ce2bb8f39c335622c3f3a7`  
		Last Modified: Wed, 31 Mar 2021 19:33:04 GMT  
		Size: 2.6 MB (2633508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0fae382c9caaf85d714725025dc973e4c111a01e3073fb71e0af12ff339d87`  
		Last Modified: Wed, 31 Mar 2021 19:33:02 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8af98c83bd092d0263be90d1ffd87110f1ec9bb32f8e33a54dfeb6ae76a5ac`  
		Last Modified: Wed, 31 Mar 2021 19:33:04 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:4cc10bfb6365d4b74f730e687c68c7a5b8bece67883b33ff42e01e8bae3e25e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8146641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb2f97da06df609bcd0734597abde0672d3dcbb6bd08049d650152d2bbf618`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:30:52 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 01 Apr 2021 13:30:55 GMT
RUN adduser -S eggdrop
# Thu, 01 Apr 2021 13:30:58 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 01 Apr 2021 13:31:01 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 01 Apr 2021 13:33:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 01 Apr 2021 13:33:02 GMT
ENV NICK=
# Thu, 01 Apr 2021 13:33:02 GMT
ENV SERVER=
# Thu, 01 Apr 2021 13:33:03 GMT
ENV LISTEN=3333
# Thu, 01 Apr 2021 13:33:04 GMT
ENV OWNER=
# Thu, 01 Apr 2021 13:33:05 GMT
ENV USERFILE=eggdrop.user
# Thu, 01 Apr 2021 13:33:06 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 01 Apr 2021 13:33:08 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 01 Apr 2021 13:33:09 GMT
EXPOSE 3333
# Thu, 01 Apr 2021 13:33:10 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 01 Apr 2021 13:33:11 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 01 Apr 2021 13:33:12 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 01 Apr 2021 13:33:13 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995fc7765c25210ac868bd04e58b22d667df8cedcfabb27eee604bd5ee6c391b`  
		Last Modified: Thu, 01 Apr 2021 13:33:48 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d5f439b8c0287a764f6cc12f616a2f58341275e4cc998ff931e780e37b3c3c`  
		Last Modified: Thu, 01 Apr 2021 13:33:46 GMT  
		Size: 10.0 KB (9996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdfc6e05825ed045492471d3a3e8c2169a1dafa8f39bdcd5ee534b4bdb081f8`  
		Last Modified: Thu, 01 Apr 2021 13:33:45 GMT  
		Size: 2.8 MB (2752494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ce691648d93fe5f23094ab687ec54a3b283c5758560b83a5076809e455830`  
		Last Modified: Thu, 01 Apr 2021 13:33:46 GMT  
		Size: 2.7 MB (2668428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364db4a48f0e41b21048c7805f35181cc08108bbfb9ffc0608f04ac644cf22bb`  
		Last Modified: Thu, 01 Apr 2021 13:33:45 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c7ad60a099a59017fd8f1bf55d4d4fb54954d9ee216cea61a5fac23a1d0798`  
		Last Modified: Thu, 01 Apr 2021 13:33:45 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
