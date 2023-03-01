## `spiped:alpine`

```console
$ docker pull spiped@sha256:946263bb4c425c1b11390f8a89fad1f052378271b0e1416df09ec3d537309a58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:alpine` - linux; amd64

```console
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:db9fbdc8e95acdd61baed85bf52d7ab004cb17dee7aa0af49efb381048c748f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d097d8022015b53fe69632c85f6ae24a781bdbbddb3e23b28bdcc34b321a5303`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 07:32:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 07:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 07:32:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 07:32:35 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 07:32:35 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 07:32:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 07:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 07:32:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65df37e068288828fdd590c704bdba0ca4a8b9872083bdcf0ed938b05bc83`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14f23472a8ad51e73644e312c9cb85c69854bc3f7259a3863b49c57f09c862`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 MB (1240903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3e94e7304b5459469fc8c8309989eaead5db21667861fb64669ab70d9611e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 206.3 KB (206329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8025107e0a863a04d24b21f3bf9d1f737abc6459904039f3c55da02f034af97`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cb12d0c5007f92277b3cf5469ce48354a5168dca26644088636f1abd9146e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:822b81d156b7c387e1ceda5cee3e6a6edd3268187a6ce26e8b85df4c68e09f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d91ebbd686f96b26164ad7739fcfca17552f6046e879f7ae2d57c3d3892739`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:18:56 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 03:18:58 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 03:18:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 03:19:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 03:19:10 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 03:19:11 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 03:19:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 03:19:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:19:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7d8401c5bd9906ab3609377e9ee6deadd5d9c4ae39ecfa8e9cd01ede0b8281`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469cab1d7427d43462f6a9628be5d2ff81ee2cd0f9f7541f9539bc00c92429f7`  
		Last Modified: Sat, 11 Feb 2023 03:19:40 GMT  
		Size: 1.5 MB (1486162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272b1229ae2f459eb6817fe20b02d6f823f26e1e8c76b8ac51eb8934b9143027`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 231.4 KB (231370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4adf5f9d6c3c73c3d7546a48714ef20383a01eeb6f321be386524c8e6e4212`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35580a675ce6a64cc7a800a1f273d54f02d5e70f9b158be76b5a569da9cdb610`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
