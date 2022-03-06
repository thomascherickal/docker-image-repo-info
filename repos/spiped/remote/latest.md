## `spiped:latest`

```console
$ docker pull spiped@sha256:5ce37d0802b83f0ec53d71d7e5a15242ce1c71396ec3991a856bffde17889365
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
$ docker pull spiped@sha256:1a1e4457b3c8d68bd9da0070e418489ba68dabb1c6dc6831f319dbaefc76a200
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37336123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8271215b728ea2bcafeb2eb89f292f11574c7e438f97173bee4e60cbf00e8f1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 09:12:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 02 Mar 2022 09:12:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 09:12:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 02 Mar 2022 09:13:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Mar 2022 09:13:02 GMT
VOLUME [/spiped]
# Wed, 02 Mar 2022 09:13:02 GMT
WORKDIR /spiped
# Wed, 02 Mar 2022 09:13:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 02 Mar 2022 09:13:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 09:13:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9a2818716d39276f9fc245a7728ebb1a31e27643ef2fa16eb96b6cebfb4d65`  
		Last Modified: Wed, 02 Mar 2022 09:13:19 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa14e3db34540d5185c56d0fbd44941e8cc18e3beaaf60f0634e18d5a705635`  
		Last Modified: Wed, 02 Mar 2022 09:13:19 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c823de0eea592fa72b002d354b7502dfa713cb2efa33858251b9220f9f06b5`  
		Last Modified: Wed, 02 Mar 2022 09:13:20 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16da16b33f377b421f18996d3c9ce41681b510405e979a524ae28497fcef8641`  
		Last Modified: Wed, 02 Mar 2022 09:13:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b986c204f9409be82e81252b1fd6de6de350596c549e9028f855a9822398860b`  
		Last Modified: Wed, 02 Mar 2022 09:13:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:058b117123d7035f5f1b09c3d22ed65d5d7d7b3effa5c3fe3b280c7176b5a765
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33940077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c0263a674511e6dc1501b4b1de9bc70017588f20f37a78d9a12a05107638b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:53 GMT
ADD file:eb61ee802e5118b26e1fec2c7fc58e34de0de54a5fd47dc6318c11a039ef528f in / 
# Tue, 01 Mar 2022 02:02:53 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 01:52:48 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 02 Mar 2022 01:52:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 01:52:58 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 02 Mar 2022 01:53:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Mar 2022 01:53:47 GMT
VOLUME [/spiped]
# Wed, 02 Mar 2022 01:53:47 GMT
WORKDIR /spiped
# Wed, 02 Mar 2022 01:53:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 02 Mar 2022 01:53:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 01:53:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4aa6e26b4dfdac27e5b5e15b7ebf4366149755a79dd653a5b68d9d93dd94c695`  
		Last Modified: Tue, 01 Mar 2022 02:18:33 GMT  
		Size: 28.9 MB (28909528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69181f76f777cff92d61dce5013d8b38a54d8a90a8139f5bfe54b98a4d2b1e1`  
		Last Modified: Wed, 02 Mar 2022 01:54:25 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0c76355da7e98e51c05bdc3ae8cfdec3d78c421113dd8c0b4cb2a90181d5bf`  
		Last Modified: Wed, 02 Mar 2022 01:54:25 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa1422462a00e06c9118cb217f46d56f701b51de3d32e45fae46b09fcff66d6`  
		Last Modified: Wed, 02 Mar 2022 01:54:29 GMT  
		Size: 5.0 MB (5027301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc521f6f085d0e490aba0dbe4c46487ef0b0585ce3e18a5f13952831153de7`  
		Last Modified: Wed, 02 Mar 2022 01:54:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53603dcc9341e834b8e42a79d3ab4e26f8d6c70859b771eb9c8edb58499775d`  
		Last Modified: Wed, 02 Mar 2022 01:54:25 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ac215edcc30b28977b317d77ccaaae94761d4354587e9800d101bb637e1149d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31315718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d7a6cecd75cfc07f7f336a43f8c0c2bd623ff9d78a61a9c7442249f5b36df1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 16:17:58 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 02 Mar 2022 16:18:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 16:18:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 02 Mar 2022 16:18:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Mar 2022 16:18:50 GMT
VOLUME [/spiped]
# Wed, 02 Mar 2022 16:18:50 GMT
WORKDIR /spiped
# Wed, 02 Mar 2022 16:18:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 02 Mar 2022 16:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 16:18:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d308a84eca5cd40a5b3b38f20aba12ad984055514266c5f21895dbd7ae398c4`  
		Last Modified: Wed, 02 Mar 2022 16:19:54 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885c743661aaee24e106ee3f2083d0acdcff80bbbfb0663485d199324303dbe2`  
		Last Modified: Wed, 02 Mar 2022 16:19:54 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b566deb17f5e2852900d444a17df344a45e23a180e0dfc06251a994ef5333c`  
		Last Modified: Wed, 02 Mar 2022 16:19:59 GMT  
		Size: 4.7 MB (4747364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f044884cf1737497ba826896f6b7e83d791a1b320f0dc816a7862caffe3d2848`  
		Last Modified: Wed, 02 Mar 2022 16:19:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e071d50afe6ad4ee58ac45ec6df078835658702fde56f4230838ffb45ed917e5`  
		Last Modified: Wed, 02 Mar 2022 16:19:54 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:1326016958abfc8116ea9f2020ecfefe12b39ab62fb59b0e5ae107af1c07b8dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35329925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007815bdb77bcdfc951019e1972a92bd8000f8b7b85c154c237ccd39b4c699d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 23:08:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 01 Mar 2022 23:08:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 23:09:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 01 Mar 2022 23:09:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 23:09:18 GMT
VOLUME [/spiped]
# Tue, 01 Mar 2022 23:09:19 GMT
WORKDIR /spiped
# Tue, 01 Mar 2022 23:09:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 01 Mar 2022 23:09:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 23:09:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95df15434040df48c54fc19d63edb9b6e713d3e57fc75371eb9bc03f439690e8`  
		Last Modified: Tue, 01 Mar 2022 23:09:49 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695632763149e2da05180caca7ea6a90ca61953988fdedce3a2606f5a1325513`  
		Last Modified: Tue, 01 Mar 2022 23:09:50 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2598a8b9ef6273d0ee0648edf9bc5383a8dfc9274cb087191db23623c8e450a`  
		Last Modified: Tue, 01 Mar 2022 23:09:50 GMT  
		Size: 5.3 MB (5269942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115fab6b17480b9dfbd15a82f115f8dfa8e35d074a58daaec4c84b2c900c764a`  
		Last Modified: Tue, 01 Mar 2022 23:09:49 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c4543827856aa8b1a91dfc23f2b7462fbb51348e324a271c9aee2b45ad46bb`  
		Last Modified: Tue, 01 Mar 2022 23:09:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:e34aca45af70e0fe79d12dbc350d533ad1f02d5079ac1e48ce22a26d785f0682
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40272088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f419d033b15cbb6cf177bc24cdce2756d0ce7a3b2b3bcdd8272717fd84d806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 04:10:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 02 Mar 2022 04:11:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 04:11:01 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 02 Mar 2022 04:11:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 02 Mar 2022 04:11:24 GMT
VOLUME [/spiped]
# Wed, 02 Mar 2022 04:11:24 GMT
WORKDIR /spiped
# Wed, 02 Mar 2022 04:11:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 02 Mar 2022 04:11:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 04:11:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ddd4bcd0c69ed3f852e2ea07a6b940c0f4e9478435c0bccbc376c13b37649`  
		Last Modified: Wed, 02 Mar 2022 04:12:01 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e745bc0d9d1edf6f7ae590350d7e9407181ce46b18f82f61e2eaf8bf0afd1e10`  
		Last Modified: Wed, 02 Mar 2022 04:12:01 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d653cf2d469bf10713ccf4014488b11752baecc3c152ed674295655ecc293fee`  
		Last Modified: Wed, 02 Mar 2022 04:12:04 GMT  
		Size: 7.9 MB (7891448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d15cba63355d98d004915f44d636604bd28abe614fb71bfd3751d6844ecebd0`  
		Last Modified: Wed, 02 Mar 2022 04:12:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33da2197ac700285791d2f9abc66232abf89e133d0cd9e9c4976b6f6e52b9889`  
		Last Modified: Wed, 02 Mar 2022 04:12:00 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:7482847668fd1ff2269e4e1bec20dd597b20ac632a62f083e7a5def10adeecb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35340855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae5cf0a64886b031443b8f8dd76059a1a4e4d64f28b6fbf4066f7273d18da5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Sat, 05 Mar 2022 17:02:53 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 05 Mar 2022 17:03:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 05 Mar 2022 17:03:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 05 Mar 2022 17:04:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 05 Mar 2022 17:04:54 GMT
VOLUME [/spiped]
# Sat, 05 Mar 2022 17:04:56 GMT
WORKDIR /spiped
# Sat, 05 Mar 2022 17:04:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 05 Mar 2022 17:05:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Mar 2022 17:05:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8655c6c15fc9046ab6f9fcb1ab2b5ba99da2fa0b0f5fb78eb6a88c8341c57`  
		Last Modified: Sat, 05 Mar 2022 17:05:21 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532ad460aab9c733a00491dbde92009091e9a27a3e91ce60d3ccba2534bf2294`  
		Last Modified: Sat, 05 Mar 2022 17:05:21 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e97e809dfeddd4ccfd05093fb0a75b0d091eec8867fb6ac58ec5af8a707b77`  
		Last Modified: Sat, 05 Mar 2022 17:05:26 GMT  
		Size: 5.7 MB (5704910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a5bdd0b59812bdf01e276165379c1cb9d6d7838b5cefddba925fd86bff6d2e`  
		Last Modified: Sat, 05 Mar 2022 17:05:21 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9269b25b6fcba7415d24fe6a96b07384dd97c0efd9d8da80e572e7bad18170`  
		Last Modified: Sat, 05 Mar 2022 17:05:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9a8ff652bffe474afdf6cf3da90bcb5fabc4674ad021bc3ddf11100309fcbe7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b89132621e69403b6931ac29ab0fdf93d27e91888256b85a1de6d142d4046a56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:15:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 22:15:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:15:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 22:17:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 22:17:09 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 22:17:12 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 22:17:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 22:17:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 22:17:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b54b67a6f99dac2db476b7702d015eb56f81c2d623bc96fd32aae703f0b732`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1241c00e00d3316ad39effb0518ce815abfcf876ea4efac9de53b2fdc560da`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ddc628c1bd5eff84e7cb044e5c93444f7e53a189710ec4b2f0213ffc82cb0f`  
		Last Modified: Wed, 26 Jan 2022 22:17:53 GMT  
		Size: 6.0 MB (5998110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706174d608bd436d8e8d5fb2c9d2cb2ff6ea71118584ab8a35af39ae43d5d90f`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7858b7298d1ed34eff1ac6724d4bce1c8fc696786a68d28c115f2bc843aad9ab`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:e4b526f6adcb1a3efedcfcb8432dbc91b2707bb29b2c9e7641de07ef960d1571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34836247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f4778f2a7ae97d8bd60c9d5b2e6301c27ea71cca10659460b408869c287754`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 13:22:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 01 Mar 2022 13:22:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 13:22:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 01 Mar 2022 13:22:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 01 Mar 2022 13:22:43 GMT
VOLUME [/spiped]
# Tue, 01 Mar 2022 13:22:43 GMT
WORKDIR /spiped
# Tue, 01 Mar 2022 13:22:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:22:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:22:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65a31fe7661db54d8076eab5e1d14fcd4b4c41eb0b404cf2ca94b64d2509662`  
		Last Modified: Tue, 01 Mar 2022 13:23:16 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b173b4c5b126e0203bf080f4a42d49989b6b60d915ce6960b9d47be83ce680`  
		Last Modified: Tue, 01 Mar 2022 13:23:16 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2d20f5e1810c5cbaf5faf137e2555c02ed0c2d4a3c856572ca948f6f7d655`  
		Last Modified: Tue, 01 Mar 2022 13:23:16 GMT  
		Size: 5.2 MB (5185865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba65cefc5c7cab67191378a849694c2900a9b4508f5449ae972d0c547437edad`  
		Last Modified: Tue, 01 Mar 2022 13:23:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec6c74b7abec32ba3d447e269c85e52a7235a6aa909c52a41ed0f6dd676e98`  
		Last Modified: Tue, 01 Mar 2022 13:23:16 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
