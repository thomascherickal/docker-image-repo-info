<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `spiped`

-	[`spiped:1`](#spiped1)
-	[`spiped:1-alpine`](#spiped1-alpine)
-	[`spiped:1.6`](#spiped16)
-	[`spiped:1.6-alpine`](#spiped16-alpine)
-	[`spiped:1.6.2`](#spiped162)
-	[`spiped:1.6.2-alpine`](#spiped162-alpine)
-	[`spiped:alpine`](#spipedalpine)
-	[`spiped:latest`](#spipedlatest)

## `spiped:1`

```console
$ docker pull spiped@sha256:33310d7c44d988ed8c41b49e7780178c30e36d5b7aea9445907efae9423d4b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1` - linux; amd64

```console
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14d854639de9f19fd5166aece1737f2390f1360015f36143f02d25c186cd0867
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a646ad837a14aa19165d093dc55b738fa61af05d383bf45142802d0b00e80ecf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 08:24:34 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 08:24:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 08:24:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 08:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 08:24:56 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 08:24:56 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 08:24:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 08:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 08:24:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff93680f513011b326d8709dea7b5823e6613c29efea3e477d537dee8d5522f`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e691ae17b64680a68f1711c3d85db162731102fdcb41a6d33c36317c5a03ef`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d817c1d15ab4cd19006f3f70a3abc0e6a743d9f729ccf9f5a8b9131c8b8864`  
		Last Modified: Wed, 16 Nov 2022 08:25:36 GMT  
		Size: 4.7 MB (4748967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2390faf6bc27ecba70c3ad7cb6f4da3f210fd34c7b460f8eac6073a17d112d`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963b2a68fab7f8a8c8fd669901c05d222a33c20248b2966a53c827908e07f529`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:15446b678eff03a766ba070afd86b1b4b2b512383e7e86ae05bdbe35761d32cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960d815e93ee6a3ba5b7e52ef354ad4259e2ad94c8cdaee91366cdac33ce10d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:25:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:25:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:25:35 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:25:35 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:25:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f263b1855bd471c83539756f8b70a58c84c9dc0ff2dbcb682afdf46fa84af`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f63490a49f76c19d7c7411339c219429156afda6ef909fcb6e4aa90b7bcbc`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90b9cb2517275e1ea4f6fa67c968e862002478d6945dd0a455d324aa9e9ef8`  
		Last Modified: Tue, 15 Nov 2022 13:25:56 GMT  
		Size: 5.3 MB (5272459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17c3ba478f87caafa84a5a1a090060c3e18cf2ef8b7000dd0294fd8c425286`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfbc8db5dc7db117e54b445680eb62aced5bdafa9c38b141250fc7aa7d5a8a`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:c473e05e698144dc8315ef89467944d3111b39a88bbad9963db8ab7843059b73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa617c4a5699ed04e207e266e667d59db1d726bba445409e8a648f5a6e4c18af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:14:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:14:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:14:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:15:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:15:44 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:15:45 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:15:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:15:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0559b9988e98911430249fdef7b998e0b4c32305f0ccd4bcb8905987488be`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b9a5754a77e47074f8f2ac4a0d9905ce7bd388dcb1f07ad8748af5ffc3e23`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7788cf8d0aadbaa693ab2c8e52e54631507aaac0f3a376941ec75476a67778a`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 5.2 MB (5188015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9f1f79d29017e6e16df8a84cd6ca4120daaabd71eecb98fce0747916d094d`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d84d4f34ee0b4bc57bc91e1c4d2b9825b124f70fe19c92c828d01c7d9325a`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e4d289144fcc0917b7c4c078e905c7eae170e8d4de2841151dabe16cd9fe14b4
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

### `spiped:1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1e0b653e4b6eedfa07996ee1e7d2e3a41cbae23c4c29b6410f1c3c08a843c249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab2799394268dbce2bd74e3feebd3689100d332af8d83cfe7484a22513fc60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:56:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:56:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:56:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:56:56 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:56:57 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:56:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e26897aae3e43075b9a0367a71b2f95b6488424bfd4663f3c6c405d7096e763`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7157993d28b1a69d4025ddcdc525d561a93315db9cc66a1b0344a71ebbd264b`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 1.5 MB (1483730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86180b4c4f5e9690553a97e5582591fa162e4c4c05db84d63d77166026b4c54c`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 231.4 KB (231390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282dbd195ef1b9176b8b02809bed658ecca6c1a8adc61249d2b82db65f5fccb`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250c8914cb765807d1d184edc38436bd02e30a85a7d66cb0632c3b4e9ee07cd`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:33310d7c44d988ed8c41b49e7780178c30e36d5b7aea9445907efae9423d4b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6` - linux; amd64

```console
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14d854639de9f19fd5166aece1737f2390f1360015f36143f02d25c186cd0867
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a646ad837a14aa19165d093dc55b738fa61af05d383bf45142802d0b00e80ecf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 08:24:34 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 08:24:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 08:24:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 08:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 08:24:56 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 08:24:56 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 08:24:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 08:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 08:24:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff93680f513011b326d8709dea7b5823e6613c29efea3e477d537dee8d5522f`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e691ae17b64680a68f1711c3d85db162731102fdcb41a6d33c36317c5a03ef`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d817c1d15ab4cd19006f3f70a3abc0e6a743d9f729ccf9f5a8b9131c8b8864`  
		Last Modified: Wed, 16 Nov 2022 08:25:36 GMT  
		Size: 4.7 MB (4748967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2390faf6bc27ecba70c3ad7cb6f4da3f210fd34c7b460f8eac6073a17d112d`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963b2a68fab7f8a8c8fd669901c05d222a33c20248b2966a53c827908e07f529`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:15446b678eff03a766ba070afd86b1b4b2b512383e7e86ae05bdbe35761d32cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960d815e93ee6a3ba5b7e52ef354ad4259e2ad94c8cdaee91366cdac33ce10d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:25:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:25:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:25:35 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:25:35 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:25:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f263b1855bd471c83539756f8b70a58c84c9dc0ff2dbcb682afdf46fa84af`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f63490a49f76c19d7c7411339c219429156afda6ef909fcb6e4aa90b7bcbc`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90b9cb2517275e1ea4f6fa67c968e862002478d6945dd0a455d324aa9e9ef8`  
		Last Modified: Tue, 15 Nov 2022 13:25:56 GMT  
		Size: 5.3 MB (5272459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17c3ba478f87caafa84a5a1a090060c3e18cf2ef8b7000dd0294fd8c425286`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfbc8db5dc7db117e54b445680eb62aced5bdafa9c38b141250fc7aa7d5a8a`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:c473e05e698144dc8315ef89467944d3111b39a88bbad9963db8ab7843059b73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa617c4a5699ed04e207e266e667d59db1d726bba445409e8a648f5a6e4c18af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:14:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:14:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:14:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:15:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:15:44 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:15:45 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:15:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:15:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0559b9988e98911430249fdef7b998e0b4c32305f0ccd4bcb8905987488be`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b9a5754a77e47074f8f2ac4a0d9905ce7bd388dcb1f07ad8748af5ffc3e23`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7788cf8d0aadbaa693ab2c8e52e54631507aaac0f3a376941ec75476a67778a`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 5.2 MB (5188015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9f1f79d29017e6e16df8a84cd6ca4120daaabd71eecb98fce0747916d094d`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d84d4f34ee0b4bc57bc91e1c4d2b9825b124f70fe19c92c828d01c7d9325a`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e4d289144fcc0917b7c4c078e905c7eae170e8d4de2841151dabe16cd9fe14b4
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

### `spiped:1.6-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1e0b653e4b6eedfa07996ee1e7d2e3a41cbae23c4c29b6410f1c3c08a843c249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab2799394268dbce2bd74e3feebd3689100d332af8d83cfe7484a22513fc60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:56:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:56:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:56:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:56:56 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:56:57 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:56:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e26897aae3e43075b9a0367a71b2f95b6488424bfd4663f3c6c405d7096e763`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7157993d28b1a69d4025ddcdc525d561a93315db9cc66a1b0344a71ebbd264b`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 1.5 MB (1483730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86180b4c4f5e9690553a97e5582591fa162e4c4c05db84d63d77166026b4c54c`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 231.4 KB (231390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282dbd195ef1b9176b8b02809bed658ecca6c1a8adc61249d2b82db65f5fccb`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250c8914cb765807d1d184edc38436bd02e30a85a7d66cb0632c3b4e9ee07cd`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:33310d7c44d988ed8c41b49e7780178c30e36d5b7aea9445907efae9423d4b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.2` - linux; amd64

```console
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14d854639de9f19fd5166aece1737f2390f1360015f36143f02d25c186cd0867
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a646ad837a14aa19165d093dc55b738fa61af05d383bf45142802d0b00e80ecf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 08:24:34 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 08:24:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 08:24:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 08:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 08:24:56 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 08:24:56 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 08:24:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 08:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 08:24:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff93680f513011b326d8709dea7b5823e6613c29efea3e477d537dee8d5522f`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e691ae17b64680a68f1711c3d85db162731102fdcb41a6d33c36317c5a03ef`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d817c1d15ab4cd19006f3f70a3abc0e6a743d9f729ccf9f5a8b9131c8b8864`  
		Last Modified: Wed, 16 Nov 2022 08:25:36 GMT  
		Size: 4.7 MB (4748967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2390faf6bc27ecba70c3ad7cb6f4da3f210fd34c7b460f8eac6073a17d112d`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963b2a68fab7f8a8c8fd669901c05d222a33c20248b2966a53c827908e07f529`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:15446b678eff03a766ba070afd86b1b4b2b512383e7e86ae05bdbe35761d32cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960d815e93ee6a3ba5b7e52ef354ad4259e2ad94c8cdaee91366cdac33ce10d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:25:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:25:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:25:35 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:25:35 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:25:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f263b1855bd471c83539756f8b70a58c84c9dc0ff2dbcb682afdf46fa84af`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f63490a49f76c19d7c7411339c219429156afda6ef909fcb6e4aa90b7bcbc`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90b9cb2517275e1ea4f6fa67c968e862002478d6945dd0a455d324aa9e9ef8`  
		Last Modified: Tue, 15 Nov 2022 13:25:56 GMT  
		Size: 5.3 MB (5272459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17c3ba478f87caafa84a5a1a090060c3e18cf2ef8b7000dd0294fd8c425286`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfbc8db5dc7db117e54b445680eb62aced5bdafa9c38b141250fc7aa7d5a8a`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:c473e05e698144dc8315ef89467944d3111b39a88bbad9963db8ab7843059b73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa617c4a5699ed04e207e266e667d59db1d726bba445409e8a648f5a6e4c18af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:14:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:14:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:14:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:15:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:15:44 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:15:45 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:15:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:15:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0559b9988e98911430249fdef7b998e0b4c32305f0ccd4bcb8905987488be`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b9a5754a77e47074f8f2ac4a0d9905ce7bd388dcb1f07ad8748af5ffc3e23`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7788cf8d0aadbaa693ab2c8e52e54631507aaac0f3a376941ec75476a67778a`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 5.2 MB (5188015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9f1f79d29017e6e16df8a84cd6ca4120daaabd71eecb98fce0747916d094d`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d84d4f34ee0b4bc57bc91e1c4d2b9825b124f70fe19c92c828d01c7d9325a`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:e4d289144fcc0917b7c4c078e905c7eae170e8d4de2841151dabe16cd9fe14b4
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

### `spiped:1.6.2-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1e0b653e4b6eedfa07996ee1e7d2e3a41cbae23c4c29b6410f1c3c08a843c249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab2799394268dbce2bd74e3feebd3689100d332af8d83cfe7484a22513fc60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:56:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:56:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:56:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:56:56 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:56:57 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:56:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e26897aae3e43075b9a0367a71b2f95b6488424bfd4663f3c6c405d7096e763`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7157993d28b1a69d4025ddcdc525d561a93315db9cc66a1b0344a71ebbd264b`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 1.5 MB (1483730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86180b4c4f5e9690553a97e5582591fa162e4c4c05db84d63d77166026b4c54c`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 231.4 KB (231390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282dbd195ef1b9176b8b02809bed658ecca6c1a8adc61249d2b82db65f5fccb`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250c8914cb765807d1d184edc38436bd02e30a85a7d66cb0632c3b4e9ee07cd`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:e4d289144fcc0917b7c4c078e905c7eae170e8d4de2841151dabe16cd9fe14b4
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
$ docker pull spiped@sha256:3e89b0e3fe93503c0766db934e147c97eb53676ea9d9c2b1e71b1f1e4f37316b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f40a8c8b2fdf3a1d59c5c833d9613a888ec1fe64ba64932df222d2e42ea664c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:57:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:57:05 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:57:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:57:16 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:57:16 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:57:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e5301aa360fa29e2207dfe75dcb69b52ecb22de2a9d32722f8dd32d16a5b17`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51504f153ef06f9d8e0efa1a12a29f40e1a37f713e7fb2912b44b1ae79f6a3f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:34 GMT  
		Size: 1.5 MB (1481753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf2dca78e48f3fde2066bbe733c1fa46d1694e6bd44106b2a875350910ddd54`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 221.3 KB (221279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460d053503b6c23d27d5ed211f692d8b8e55caf75003ef3450c8b246d6f6d000`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52159807c1a836f1ffdb8f6a44d89972dfd5fd16c446f652cf31c259b78f6f4`  
		Last Modified: Thu, 01 Dec 2022 19:57:33 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:c4b7b9389704094c8e559d092f3ff46dd5c9cadcb6e101deaf38496862015620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604cc9ff9561d020924d116aa1d088c57973f082455d55d79c9020af5e0da3ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:49:45 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:49:46 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:49:46 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:49:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:49:55 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:49:55 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:49:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:49:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4465a6ed0bd7daa721e08fd7417d8f953e45121ba61bdf871d1e8d62bdcd27`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9ad950888f95a4002dda2bb274489a2bee29c851d750a75d3b3c653ad3fff`  
		Last Modified: Thu, 01 Dec 2022 19:50:18 GMT  
		Size: 1.2 MB (1238919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a500025ba958493ecce30c80b43bf227d405c78cd7c805d549858f3beeb5fe70`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 206.3 KB (206332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a947285b2d494f975075fd5472b0b71d8b445b7cabe2d9b994959024575c741`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98f8d905f70d030edf6be459671c6b5b48f3a2002bca98770deed66ec3ffa7`  
		Last Modified: Thu, 01 Dec 2022 19:50:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e4ef2c928d40fb9e522649dd49f9f647b2421138cce20e200c1b15f7aa715684
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb34800255ac012f06c688d0421f93b3b51947ea56e4a4b1d4b5aceb66260504`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:25:26 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:25:29 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:25:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:25:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:25:37 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:25:37 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:25:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:25:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ecaf8dbf0b2c4e30443a511b9611f79a60212efd36edf5aff69f9294d5378`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15afb355281d113b775bc114ed9b27f025bfadc199a4971604ba53d673beae2`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 1.2 MB (1166542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e86d60e87d2fa5e55ae348fe2faafad4cd216f2331c6a53a01da63fac289629`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 200.1 KB (200090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ed2a16261026fd134e3e2e7b943142552508b42f378a9aa0ce4a86cba0977`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ff4a0f0d6e04aba68e5d89095f445ca82664968213a6dbe99a6e33e747b28`  
		Last Modified: Thu, 01 Dec 2022 20:26:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:5e7f3bf4785acfd947bf700dd6af7285a49437dcc048e193324e6c4e1f0a65d1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40662536621d39a5d1d56b36264773a35ad4b9502eedad9a2672e9d24bd5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:22:42 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:22:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:22:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:22:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:22:52 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:22:52 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:22:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:22:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc49f2ca67d5973f8e4918aabaff56d682b74c556ceebf188d8eb35a4c5b49`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902ba991cb46c2e24b6a4023949820ed34b471fb521e4343bdadf6cbd9c90d9f`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 1.4 MB (1362326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bbe2790fbd90d89444fda5085bbfc9ff80949c274408ae5f1de5f6ba9a616`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 215.7 KB (215687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15606d60b1d5f10fb36fa9beaf12df582957c07f17618adbfb328e35e425d632`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3708f7957add5299aef760297a84038a0ef8d22113dfe41ad65056972f7aab86`  
		Last Modified: Thu, 01 Dec 2022 20:23:10 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:1e0b653e4b6eedfa07996ee1e7d2e3a41cbae23c4c29b6410f1c3c08a843c249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ab2799394268dbce2bd74e3feebd3689100d332af8d83cfe7484a22513fc60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:56:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:56:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:56:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:56:56 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:56:57 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:56:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e26897aae3e43075b9a0367a71b2f95b6488424bfd4663f3c6c405d7096e763`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7157993d28b1a69d4025ddcdc525d561a93315db9cc66a1b0344a71ebbd264b`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 1.5 MB (1483730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86180b4c4f5e9690553a97e5582591fa162e4c4c05db84d63d77166026b4c54c`  
		Last Modified: Thu, 01 Dec 2022 19:57:29 GMT  
		Size: 231.4 KB (231390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0282dbd195ef1b9176b8b02809bed658ecca6c1a8adc61249d2b82db65f5fccb`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250c8914cb765807d1d184edc38436bd02e30a85a7d66cb0632c3b4e9ee07cd`  
		Last Modified: Thu, 01 Dec 2022 19:57:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:0d82c8ddd4037c340c7f34bc6e73db3214b03515efcd874588bc3365ac085bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28944c47eb88aee8f3a553a774aba1a3fd620bf05ab8e15e7a7d681520f5d215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:50:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 19:50:44 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 19:50:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 19:50:59 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 19:51:00 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 19:51:00 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 19:51:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 19:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:51:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5433922e50398442c5441e700ce384e59f342ba21344c1ca15266cf077e73d80`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1e29ac9af1e4bf31e1b576203c2580e68c391fd4400acd52c3707cf5d28bcd`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 1.4 MB (1411369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd56ef26bfb6ed677e16a67c99173ef8cee0cb3982f66da97ea0230c8959a2d`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 220.0 KB (220032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e77aa3f9e366961824c7e77c1800d988c6f9ef1f5e4cc36d4bba2d106dfed9`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9b1af69786ab6ff98fd2b2ff2c4d0a598abff43f13482a144b6f55aaa571f`  
		Last Modified: Thu, 01 Dec 2022 19:51:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:f94963d593297b0a6d16d71b3a958d319f35f32ae69478af40499ff0f4f232ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71b4c3c79f61cf77f40c85b0da2db41488517dce6c0411120e2b6d067b45a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 20:08:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 01 Dec 2022 20:08:03 GMT
RUN apk add --no-cache libssl1.1
# Thu, 01 Dec 2022 20:08:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 01 Dec 2022 20:08:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 01 Dec 2022 20:08:09 GMT
VOLUME [/spiped]
# Thu, 01 Dec 2022 20:08:10 GMT
WORKDIR /spiped
# Thu, 01 Dec 2022 20:08:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 01 Dec 2022 20:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 20:08:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52148273cd46ffe35fedaf18c26097356ca859da825c5b8208d5b63e0a49a9d`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94da62a786e1774b7e939895037d72a10a2e0dc599c52c5a24569e7cf6050abc`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 1.2 MB (1221160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90131fd2254dc50bbf637f22b04446ad23c469439bab9c004b73582cde15c009`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 208.6 KB (208635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5696b5c9d9179914c43687bc60cb6adda2b93e14f0c28c85185be55213a0da5`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da71b6653ae36e91be45313442a413808b08cd20ec26976860212182ed4d77`  
		Last Modified: Thu, 01 Dec 2022 20:08:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:33310d7c44d988ed8c41b49e7780178c30e36d5b7aea9445907efae9423d4b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:latest` - linux; amd64

```console
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14d854639de9f19fd5166aece1737f2390f1360015f36143f02d25c186cd0867
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a646ad837a14aa19165d093dc55b738fa61af05d383bf45142802d0b00e80ecf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 08:24:34 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 08:24:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 08:24:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 08:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 08:24:56 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 08:24:56 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 08:24:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 08:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 08:24:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff93680f513011b326d8709dea7b5823e6613c29efea3e477d537dee8d5522f`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e691ae17b64680a68f1711c3d85db162731102fdcb41a6d33c36317c5a03ef`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d817c1d15ab4cd19006f3f70a3abc0e6a743d9f729ccf9f5a8b9131c8b8864`  
		Last Modified: Wed, 16 Nov 2022 08:25:36 GMT  
		Size: 4.7 MB (4748967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2390faf6bc27ecba70c3ad7cb6f4da3f210fd34c7b460f8eac6073a17d112d`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963b2a68fab7f8a8c8fd669901c05d222a33c20248b2966a53c827908e07f529`  
		Last Modified: Wed, 16 Nov 2022 08:25:35 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:15446b678eff03a766ba070afd86b1b4b2b512383e7e86ae05bdbe35761d32cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35336319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960d815e93ee6a3ba5b7e52ef354ad4259e2ad94c8cdaee91366cdac33ce10d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:25:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:25:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:25:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:25:35 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:25:35 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:25:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f263b1855bd471c83539756f8b70a58c84c9dc0ff2dbcb682afdf46fa84af`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f63490a49f76c19d7c7411339c219429156afda6ef909fcb6e4aa90b7bcbc`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90b9cb2517275e1ea4f6fa67c968e862002478d6945dd0a455d324aa9e9ef8`  
		Last Modified: Tue, 15 Nov 2022 13:25:56 GMT  
		Size: 5.3 MB (5272459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17c3ba478f87caafa84a5a1a090060c3e18cf2ef8b7000dd0294fd8c425286`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bfbc8db5dc7db117e54b445680eb62aced5bdafa9c38b141250fc7aa7d5a8a`  
		Last Modified: Tue, 15 Nov 2022 13:25:55 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:c473e05e698144dc8315ef89467944d3111b39a88bbad9963db8ab7843059b73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa617c4a5699ed04e207e266e667d59db1d726bba445409e8a648f5a6e4c18af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:14:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 13:14:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:14:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 13:15:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 13:15:44 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 13:15:45 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 13:15:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:15:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0559b9988e98911430249fdef7b998e0b4c32305f0ccd4bcb8905987488be`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b9a5754a77e47074f8f2ac4a0d9905ce7bd388dcb1f07ad8748af5ffc3e23`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7788cf8d0aadbaa693ab2c8e52e54631507aaac0f3a376941ec75476a67778a`  
		Last Modified: Tue, 15 Nov 2022 13:16:33 GMT  
		Size: 5.2 MB (5188015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9f1f79d29017e6e16df8a84cd6ca4120daaabd71eecb98fce0747916d094d`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d84d4f34ee0b4bc57bc91e1c4d2b9825b124f70fe19c92c828d01c7d9325a`  
		Last Modified: Tue, 15 Nov 2022 13:16:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
