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
$ docker pull spiped@sha256:1d577045d45b0ae89721417ce0ff12570df1a60bdfd748dd9ece51cf4a9ab0bd
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
$ docker pull spiped@sha256:80b3e8ee4628829b3e7808844f5491d7f5a428fdf34b222f015a585458fd6f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37398423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7988b8379fddac2783b6ba47c03be52fd318c7d8a15dc38a46be7959eccd9d24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:35:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 13:35:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 13:35:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 13:35:33 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 13:35:33 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 13:35:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 13:35:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb43ec866fe3cc317a36fa75d6ec2cfaecbf61259805e686134135c2feb7b2b`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b847f081ab25a6a60a0f9227658a9ed04ca809493ef1c23370f819960fae4bf9`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440a618898e824f0daa5b9e12c764cfa879588620c3bee3b56d387ba756975c6`  
		Last Modified: Sat, 04 Feb 2023 13:35:51 GMT  
		Size: 6.0 MB (5998255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395c945c21da9e37967288c6017ab0ba47b905a00c659e8c31051f77c9203ecc`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45038da82a8a6524ba8d5a36b01c7a21b85e45394fa51148b68b43658739b9c7`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:883367b70f604d047a082cc4f152f3f4f802288402e3722ce365f1f6c59bad07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33930181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ad7e21ecfa7a20adac9a632da3ad3ad473a297d33eb155fe7d2ed3bff9e682`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:38 GMT
ADD file:ce468627e54d8d1c839cea8ab62e505f612298fd97d50e189293fcfcc6af03a5 in / 
# Sat, 04 Feb 2023 02:46:38 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:01:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 10:01:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:01:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 10:02:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:02:02 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 10:02:03 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 10:02:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 10:02:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:83735a64f458d40820e4310d632e8bb1dc888f6c25114496be3ce431b5f21d5d`  
		Last Modified: Sat, 04 Feb 2023 02:51:43 GMT  
		Size: 28.9 MB (28898637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bdfb7b24b8646ef452836b9abcc4c73c0b7f55202ffa710d2bfaa65bc3aa1`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326bd6c277911d1d0cfa04ad295df1221e1fa32219c63d53f206cff44c355972`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f46b32e187e216348661375893cbc04fdb397813ccba4bdc9679db4824720`  
		Last Modified: Sat, 04 Feb 2023 10:02:21 GMT  
		Size: 5.0 MB (5028361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52724ebfc8187d2778a989c84f0be4e017eea25ad3ef2cff5d818452ba97cee3`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1834f6fe2aa9fd01acc280547a4ed704342f7ac354b6d8c407911380a787dff0`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ff2d37d643dba46ec1ca3f190136140c2039c88ce18c8c3c1cda35f75841cd7b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa13aea4e448660a02807e09e9f129b075ddcd15f4f5207e4a1d5c5ebfa02de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:17:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 21:17:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:17:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 21:18:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 21:18:16 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 21:18:16 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 21:18:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:18:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 21:18:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343813fba016b62cf17ebead34dba4d1126a460796db3fb269bebbd3fe2cdd01`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45570ed34e4ad5a6ea26a074f5aac8422e806304219c4b46a060487b4f28b5`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f648b1f6094ef5bd0966d575b58cc91b17e6313884799f5d38b8d591562127a`  
		Last Modified: Sat, 04 Feb 2023 21:18:54 GMT  
		Size: 4.7 MB (4748967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8963d89184feb68cbf98f295746b3544bbd9caa800dd9e59f2a8e7bff44cc1d`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a250310debb236e8572275069607e0465c91d2c1db38ea09bfc4176dcbe42`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:e99ea9f84c5e7227931a654635c48c2412677415cf41f22e9cfaf34891c29ff7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35320612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0306e8774f16019968e446127b379b0d1696e2cac8d17b7e0168198cdb22e2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:45:22 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 17:45:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:45:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 17:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:45:42 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 17:45:42 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 17:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e0bfebbe73df67f67a93f5cbb234e1280ccce0f38bd5afa6d69af18cc7cacd`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943241ea7d66696ea790525f04d919838ab68408d32c67ef6e6a1d87f0808b02`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60dfd4f224ba8c244ec6b8489cfada1dff311fab9c3de9c10335d009e99c637d`  
		Last Modified: Sat, 04 Feb 2023 17:45:58 GMT  
		Size: 5.3 MB (5272564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4ddd6c193d40bfbdafb184d07f66eeecd27589a446d6d4e2b33d3e3533a53`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a476866dbd7db5b6a17bcfd9b21f41336bd255c7feb0bee8a8445df77a2c2033`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:3b5039822964df0400c1c464337e7eb24a76e514762eecf8266356c255a8bc20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40269264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9365baff0a3fb27f1f66b81d2a56556b6bd2c28306db3172f2c38d67541c62a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:37:03 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 21:37:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:37:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 21:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 21:37:29 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 21:37:30 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 21:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:37:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 21:37:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283c04967521e536e9cf08d98eb23ae5ad68d198149c30398cde479eb3fab5e9`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af281af24ba85838614da7407d24c208b44b74cff7983143ad92830dad38133`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf2fb585912d154cc8f37a974f45e7282c72ab0ddd491c0f49bb3fd8acfe30`  
		Last Modified: Sat, 04 Feb 2023 21:38:02 GMT  
		Size: 7.9 MB (7890521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1d975756e334c454f6b84b9a3dc6fbc07f5917a15e139408a47515bd364d79`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5442e2600347208e73136ad766df54a7c9fdfeb85ebaabc9c55fa6dd3dbeaecd`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:b730466434599fad0c0b7f45842928f46d35b73a8aeaface9fb6ec3b163a8942
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7df08512320dac74f33c923af82d12788d3060be6c84905071a5ffafaaecb15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 Jan 2023 16:34:24 GMT
ADD file:295faaf493f6a8d3e2a3eecb28c8f5ac765a1281656221d0a3ab482312a5ee28 in / 
# Wed, 11 Jan 2023 16:34:29 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 02:33:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 Jan 2023 02:34:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 02:34:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 Jan 2023 02:35:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 Jan 2023 02:35:49 GMT
VOLUME [/spiped]
# Thu, 12 Jan 2023 02:35:52 GMT
WORKDIR /spiped
# Thu, 12 Jan 2023 02:35:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 Jan 2023 02:35:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Jan 2023 02:35:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9d653aeb7081a0b221d1160bd67b030696ca49b7ca91912bf298835f8f75ac7b`  
		Last Modified: Wed, 11 Jan 2023 16:43:17 GMT  
		Size: 29.6 MB (29619870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abe6f03d096edad9cefbcccc088c938e23a7055d4351e8cfeb37aa5787fb436`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f896ed2d956a527e2710b5814c6c336e0ced9a98209fcd3432f2dd10b6b67`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d27e290b4bfbefbe11ef090278d14200ce78aae72f617a0c45b72196694ec6`  
		Last Modified: Thu, 12 Jan 2023 02:36:28 GMT  
		Size: 5.7 MB (5705001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95502918743e976e174ed1430de13433c908c65971251adc0941ed528de608f3`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ec717daf1fdf53be4cb1236d04557051ce2dbbf0239b4bbe63b835eb3dd9af`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:30875847cb61b6e1e9f3b5ef6700a0d0eaeee0fdbe93d9844aadf8e286f45472
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41271646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e663c415cbc813e4455e17f82e9126ad10b3ce41a1a913f8e3c7c4bedff18979`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:15:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 17:15:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:15:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 17:16:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:16:05 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 17:16:05 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 17:16:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:16:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:16:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfbdb5fc624191d3f46fae3517ddc1d9e13099a128f28c9c072bc90ec1544dc`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778da259d3954937b144a1302513548989f72feacb6e03870d9ac49002541911`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78952c4b6fad0cc7a3dc3cc41e933cd84346f3b54fe8ec183e7316c0b7087bb9`  
		Last Modified: Sat, 04 Feb 2023 17:16:44 GMT  
		Size: 6.0 MB (5999596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0908ade9b64212309ad3d33772064d6b1be92c2cd3a30c09886eb718fdfec250`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeec2b6d00157ae684bb6c4a1d08d28bf4a0a98c5ee968e5d85e7af5f0ec930`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:ce90d8c9c4121874af31c7fb7f2b625d61671dd1a95ce7c32e652d202cbb546b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34820311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91ddadcd9b85198af8fd4ceb73151e93cb79de37b0a5b31d7259deb2d70116c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:15 GMT
ADD file:29a3ecb38611dbbb6f45b2d10ad3cee60c0198429376f999e9a397f9c405820e in / 
# Sat, 04 Feb 2023 04:06:17 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 08:49:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 08:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:49:18 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 08:49:18 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 08:49:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:49:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c6fe4d1ef15da79055e0a71952e1a38f799d4f36e9acebdb1ec1512651b39f1`  
		Last Modified: Sat, 04 Feb 2023 04:10:27 GMT  
		Size: 29.6 MB (29629678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dc1bc8bba5799858fb508b0c9f5a42fea7a6c0c9eb8de3b35db1d973fc6d9e`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0706fd31877fe4e89e6f262040926d1ba14e7b7fa79f0dcae19ae4e31f3f`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32c2abc910e11be92a564001147caa29ce390b91f354136cbbfb5203c31d0a9`  
		Last Modified: Sat, 04 Feb 2023 08:49:49 GMT  
		Size: 5.2 MB (5187378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6169f704622be973593aff410bf27a3c9ec307c98ded94cd405c8a6c2e09e7`  
		Last Modified: Sat, 04 Feb 2023 08:49:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04839df6cf6945726323210131a6af490b1cec7f3a2d959e8cd96d95dc9bd0b7`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e8982ce4c33ed5c5fdf992ccf6c890b82d7806e41d8778ea6777610d0e4e4719
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
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5a87be0c5f3e288adf33abd9c67087730cd729e12ac28ae4b107955683edff20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63961a94a731d4f9e0005f5fd83043126c5546496fa856ea125a5c2e51c6979c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:32:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:32:52 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:32:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:33:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:33:02 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:33:03 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:33:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:33:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f659d5259c21b4ce33d18c83c0251b9d66d58281847f63904bed75a5683b3fde`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decaf35186276ee535aac72c69938baded768609a2bb148ca4d5c0a1788a984`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.2 MB (1221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93194a8cc16c2fcd24da284630284cd3fbf877fc323c8dc65e3d256d777ac04a`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 208.6 KB (208637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02decf839b354e56295448b1f40e50f813a1879598a091e766908a8f70b21671`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2035a6bfb730bee20ac317d153b1061a4002ce6a450bb74f34bebcfa04369`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:1d577045d45b0ae89721417ce0ff12570df1a60bdfd748dd9ece51cf4a9ab0bd
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
$ docker pull spiped@sha256:80b3e8ee4628829b3e7808844f5491d7f5a428fdf34b222f015a585458fd6f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37398423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7988b8379fddac2783b6ba47c03be52fd318c7d8a15dc38a46be7959eccd9d24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:35:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 13:35:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 13:35:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 13:35:33 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 13:35:33 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 13:35:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 13:35:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb43ec866fe3cc317a36fa75d6ec2cfaecbf61259805e686134135c2feb7b2b`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b847f081ab25a6a60a0f9227658a9ed04ca809493ef1c23370f819960fae4bf9`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440a618898e824f0daa5b9e12c764cfa879588620c3bee3b56d387ba756975c6`  
		Last Modified: Sat, 04 Feb 2023 13:35:51 GMT  
		Size: 6.0 MB (5998255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395c945c21da9e37967288c6017ab0ba47b905a00c659e8c31051f77c9203ecc`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45038da82a8a6524ba8d5a36b01c7a21b85e45394fa51148b68b43658739b9c7`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:883367b70f604d047a082cc4f152f3f4f802288402e3722ce365f1f6c59bad07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33930181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ad7e21ecfa7a20adac9a632da3ad3ad473a297d33eb155fe7d2ed3bff9e682`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:38 GMT
ADD file:ce468627e54d8d1c839cea8ab62e505f612298fd97d50e189293fcfcc6af03a5 in / 
# Sat, 04 Feb 2023 02:46:38 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:01:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 10:01:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:01:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 10:02:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:02:02 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 10:02:03 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 10:02:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 10:02:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:83735a64f458d40820e4310d632e8bb1dc888f6c25114496be3ce431b5f21d5d`  
		Last Modified: Sat, 04 Feb 2023 02:51:43 GMT  
		Size: 28.9 MB (28898637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bdfb7b24b8646ef452836b9abcc4c73c0b7f55202ffa710d2bfaa65bc3aa1`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326bd6c277911d1d0cfa04ad295df1221e1fa32219c63d53f206cff44c355972`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f46b32e187e216348661375893cbc04fdb397813ccba4bdc9679db4824720`  
		Last Modified: Sat, 04 Feb 2023 10:02:21 GMT  
		Size: 5.0 MB (5028361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52724ebfc8187d2778a989c84f0be4e017eea25ad3ef2cff5d818452ba97cee3`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1834f6fe2aa9fd01acc280547a4ed704342f7ac354b6d8c407911380a787dff0`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ff2d37d643dba46ec1ca3f190136140c2039c88ce18c8c3c1cda35f75841cd7b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa13aea4e448660a02807e09e9f129b075ddcd15f4f5207e4a1d5c5ebfa02de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:17:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 21:17:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:17:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 21:18:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 21:18:16 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 21:18:16 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 21:18:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:18:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 21:18:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343813fba016b62cf17ebead34dba4d1126a460796db3fb269bebbd3fe2cdd01`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45570ed34e4ad5a6ea26a074f5aac8422e806304219c4b46a060487b4f28b5`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f648b1f6094ef5bd0966d575b58cc91b17e6313884799f5d38b8d591562127a`  
		Last Modified: Sat, 04 Feb 2023 21:18:54 GMT  
		Size: 4.7 MB (4748967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8963d89184feb68cbf98f295746b3544bbd9caa800dd9e59f2a8e7bff44cc1d`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a250310debb236e8572275069607e0465c91d2c1db38ea09bfc4176dcbe42`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:e99ea9f84c5e7227931a654635c48c2412677415cf41f22e9cfaf34891c29ff7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35320612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0306e8774f16019968e446127b379b0d1696e2cac8d17b7e0168198cdb22e2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:45:22 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 17:45:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:45:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 17:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:45:42 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 17:45:42 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 17:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e0bfebbe73df67f67a93f5cbb234e1280ccce0f38bd5afa6d69af18cc7cacd`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943241ea7d66696ea790525f04d919838ab68408d32c67ef6e6a1d87f0808b02`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60dfd4f224ba8c244ec6b8489cfada1dff311fab9c3de9c10335d009e99c637d`  
		Last Modified: Sat, 04 Feb 2023 17:45:58 GMT  
		Size: 5.3 MB (5272564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4ddd6c193d40bfbdafb184d07f66eeecd27589a446d6d4e2b33d3e3533a53`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a476866dbd7db5b6a17bcfd9b21f41336bd255c7feb0bee8a8445df77a2c2033`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:3b5039822964df0400c1c464337e7eb24a76e514762eecf8266356c255a8bc20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40269264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9365baff0a3fb27f1f66b81d2a56556b6bd2c28306db3172f2c38d67541c62a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:37:03 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 21:37:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:37:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 21:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 21:37:29 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 21:37:30 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 21:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:37:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 21:37:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283c04967521e536e9cf08d98eb23ae5ad68d198149c30398cde479eb3fab5e9`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af281af24ba85838614da7407d24c208b44b74cff7983143ad92830dad38133`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf2fb585912d154cc8f37a974f45e7282c72ab0ddd491c0f49bb3fd8acfe30`  
		Last Modified: Sat, 04 Feb 2023 21:38:02 GMT  
		Size: 7.9 MB (7890521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1d975756e334c454f6b84b9a3dc6fbc07f5917a15e139408a47515bd364d79`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5442e2600347208e73136ad766df54a7c9fdfeb85ebaabc9c55fa6dd3dbeaecd`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:b730466434599fad0c0b7f45842928f46d35b73a8aeaface9fb6ec3b163a8942
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7df08512320dac74f33c923af82d12788d3060be6c84905071a5ffafaaecb15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 Jan 2023 16:34:24 GMT
ADD file:295faaf493f6a8d3e2a3eecb28c8f5ac765a1281656221d0a3ab482312a5ee28 in / 
# Wed, 11 Jan 2023 16:34:29 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 02:33:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 Jan 2023 02:34:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 02:34:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 Jan 2023 02:35:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 Jan 2023 02:35:49 GMT
VOLUME [/spiped]
# Thu, 12 Jan 2023 02:35:52 GMT
WORKDIR /spiped
# Thu, 12 Jan 2023 02:35:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 Jan 2023 02:35:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Jan 2023 02:35:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9d653aeb7081a0b221d1160bd67b030696ca49b7ca91912bf298835f8f75ac7b`  
		Last Modified: Wed, 11 Jan 2023 16:43:17 GMT  
		Size: 29.6 MB (29619870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abe6f03d096edad9cefbcccc088c938e23a7055d4351e8cfeb37aa5787fb436`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f896ed2d956a527e2710b5814c6c336e0ced9a98209fcd3432f2dd10b6b67`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d27e290b4bfbefbe11ef090278d14200ce78aae72f617a0c45b72196694ec6`  
		Last Modified: Thu, 12 Jan 2023 02:36:28 GMT  
		Size: 5.7 MB (5705001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95502918743e976e174ed1430de13433c908c65971251adc0941ed528de608f3`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ec717daf1fdf53be4cb1236d04557051ce2dbbf0239b4bbe63b835eb3dd9af`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:30875847cb61b6e1e9f3b5ef6700a0d0eaeee0fdbe93d9844aadf8e286f45472
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41271646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e663c415cbc813e4455e17f82e9126ad10b3ce41a1a913f8e3c7c4bedff18979`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:15:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 17:15:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:15:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 17:16:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:16:05 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 17:16:05 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 17:16:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:16:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:16:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfbdb5fc624191d3f46fae3517ddc1d9e13099a128f28c9c072bc90ec1544dc`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778da259d3954937b144a1302513548989f72feacb6e03870d9ac49002541911`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78952c4b6fad0cc7a3dc3cc41e933cd84346f3b54fe8ec183e7316c0b7087bb9`  
		Last Modified: Sat, 04 Feb 2023 17:16:44 GMT  
		Size: 6.0 MB (5999596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0908ade9b64212309ad3d33772064d6b1be92c2cd3a30c09886eb718fdfec250`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeec2b6d00157ae684bb6c4a1d08d28bf4a0a98c5ee968e5d85e7af5f0ec930`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:ce90d8c9c4121874af31c7fb7f2b625d61671dd1a95ce7c32e652d202cbb546b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34820311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91ddadcd9b85198af8fd4ceb73151e93cb79de37b0a5b31d7259deb2d70116c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:15 GMT
ADD file:29a3ecb38611dbbb6f45b2d10ad3cee60c0198429376f999e9a397f9c405820e in / 
# Sat, 04 Feb 2023 04:06:17 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 08:49:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 08:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:49:18 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 08:49:18 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 08:49:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:49:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c6fe4d1ef15da79055e0a71952e1a38f799d4f36e9acebdb1ec1512651b39f1`  
		Last Modified: Sat, 04 Feb 2023 04:10:27 GMT  
		Size: 29.6 MB (29629678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dc1bc8bba5799858fb508b0c9f5a42fea7a6c0c9eb8de3b35db1d973fc6d9e`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0706fd31877fe4e89e6f262040926d1ba14e7b7fa79f0dcae19ae4e31f3f`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32c2abc910e11be92a564001147caa29ce390b91f354136cbbfb5203c31d0a9`  
		Last Modified: Sat, 04 Feb 2023 08:49:49 GMT  
		Size: 5.2 MB (5187378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6169f704622be973593aff410bf27a3c9ec307c98ded94cd405c8a6c2e09e7`  
		Last Modified: Sat, 04 Feb 2023 08:49:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04839df6cf6945726323210131a6af490b1cec7f3a2d959e8cd96d95dc9bd0b7`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e8982ce4c33ed5c5fdf992ccf6c890b82d7806e41d8778ea6777610d0e4e4719
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
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5a87be0c5f3e288adf33abd9c67087730cd729e12ac28ae4b107955683edff20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63961a94a731d4f9e0005f5fd83043126c5546496fa856ea125a5c2e51c6979c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:32:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:32:52 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:32:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:33:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:33:02 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:33:03 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:33:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:33:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f659d5259c21b4ce33d18c83c0251b9d66d58281847f63904bed75a5683b3fde`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decaf35186276ee535aac72c69938baded768609a2bb148ca4d5c0a1788a984`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.2 MB (1221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93194a8cc16c2fcd24da284630284cd3fbf877fc323c8dc65e3d256d777ac04a`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 208.6 KB (208637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02decf839b354e56295448b1f40e50f813a1879598a091e766908a8f70b21671`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2035a6bfb730bee20ac317d153b1061a4002ce6a450bb74f34bebcfa04369`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:1d577045d45b0ae89721417ce0ff12570df1a60bdfd748dd9ece51cf4a9ab0bd
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
$ docker pull spiped@sha256:80b3e8ee4628829b3e7808844f5491d7f5a428fdf34b222f015a585458fd6f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37398423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7988b8379fddac2783b6ba47c03be52fd318c7d8a15dc38a46be7959eccd9d24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:35:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 13:35:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 13:35:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 13:35:33 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 13:35:33 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 13:35:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 13:35:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb43ec866fe3cc317a36fa75d6ec2cfaecbf61259805e686134135c2feb7b2b`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b847f081ab25a6a60a0f9227658a9ed04ca809493ef1c23370f819960fae4bf9`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440a618898e824f0daa5b9e12c764cfa879588620c3bee3b56d387ba756975c6`  
		Last Modified: Sat, 04 Feb 2023 13:35:51 GMT  
		Size: 6.0 MB (5998255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395c945c21da9e37967288c6017ab0ba47b905a00c659e8c31051f77c9203ecc`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45038da82a8a6524ba8d5a36b01c7a21b85e45394fa51148b68b43658739b9c7`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:883367b70f604d047a082cc4f152f3f4f802288402e3722ce365f1f6c59bad07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33930181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ad7e21ecfa7a20adac9a632da3ad3ad473a297d33eb155fe7d2ed3bff9e682`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:38 GMT
ADD file:ce468627e54d8d1c839cea8ab62e505f612298fd97d50e189293fcfcc6af03a5 in / 
# Sat, 04 Feb 2023 02:46:38 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:01:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 10:01:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:01:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 10:02:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:02:02 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 10:02:03 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 10:02:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 10:02:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:83735a64f458d40820e4310d632e8bb1dc888f6c25114496be3ce431b5f21d5d`  
		Last Modified: Sat, 04 Feb 2023 02:51:43 GMT  
		Size: 28.9 MB (28898637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bdfb7b24b8646ef452836b9abcc4c73c0b7f55202ffa710d2bfaa65bc3aa1`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326bd6c277911d1d0cfa04ad295df1221e1fa32219c63d53f206cff44c355972`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f46b32e187e216348661375893cbc04fdb397813ccba4bdc9679db4824720`  
		Last Modified: Sat, 04 Feb 2023 10:02:21 GMT  
		Size: 5.0 MB (5028361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52724ebfc8187d2778a989c84f0be4e017eea25ad3ef2cff5d818452ba97cee3`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1834f6fe2aa9fd01acc280547a4ed704342f7ac354b6d8c407911380a787dff0`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ff2d37d643dba46ec1ca3f190136140c2039c88ce18c8c3c1cda35f75841cd7b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa13aea4e448660a02807e09e9f129b075ddcd15f4f5207e4a1d5c5ebfa02de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:17:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 21:17:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:17:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 21:18:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 21:18:16 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 21:18:16 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 21:18:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:18:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 21:18:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343813fba016b62cf17ebead34dba4d1126a460796db3fb269bebbd3fe2cdd01`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45570ed34e4ad5a6ea26a074f5aac8422e806304219c4b46a060487b4f28b5`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f648b1f6094ef5bd0966d575b58cc91b17e6313884799f5d38b8d591562127a`  
		Last Modified: Sat, 04 Feb 2023 21:18:54 GMT  
		Size: 4.7 MB (4748967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8963d89184feb68cbf98f295746b3544bbd9caa800dd9e59f2a8e7bff44cc1d`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a250310debb236e8572275069607e0465c91d2c1db38ea09bfc4176dcbe42`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:e99ea9f84c5e7227931a654635c48c2412677415cf41f22e9cfaf34891c29ff7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35320612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0306e8774f16019968e446127b379b0d1696e2cac8d17b7e0168198cdb22e2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:45:22 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 17:45:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:45:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 17:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:45:42 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 17:45:42 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 17:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e0bfebbe73df67f67a93f5cbb234e1280ccce0f38bd5afa6d69af18cc7cacd`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943241ea7d66696ea790525f04d919838ab68408d32c67ef6e6a1d87f0808b02`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60dfd4f224ba8c244ec6b8489cfada1dff311fab9c3de9c10335d009e99c637d`  
		Last Modified: Sat, 04 Feb 2023 17:45:58 GMT  
		Size: 5.3 MB (5272564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4ddd6c193d40bfbdafb184d07f66eeecd27589a446d6d4e2b33d3e3533a53`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a476866dbd7db5b6a17bcfd9b21f41336bd255c7feb0bee8a8445df77a2c2033`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:3b5039822964df0400c1c464337e7eb24a76e514762eecf8266356c255a8bc20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40269264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9365baff0a3fb27f1f66b81d2a56556b6bd2c28306db3172f2c38d67541c62a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:37:03 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 21:37:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:37:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 21:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 21:37:29 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 21:37:30 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 21:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:37:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 21:37:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283c04967521e536e9cf08d98eb23ae5ad68d198149c30398cde479eb3fab5e9`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af281af24ba85838614da7407d24c208b44b74cff7983143ad92830dad38133`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf2fb585912d154cc8f37a974f45e7282c72ab0ddd491c0f49bb3fd8acfe30`  
		Last Modified: Sat, 04 Feb 2023 21:38:02 GMT  
		Size: 7.9 MB (7890521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1d975756e334c454f6b84b9a3dc6fbc07f5917a15e139408a47515bd364d79`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5442e2600347208e73136ad766df54a7c9fdfeb85ebaabc9c55fa6dd3dbeaecd`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:b730466434599fad0c0b7f45842928f46d35b73a8aeaface9fb6ec3b163a8942
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7df08512320dac74f33c923af82d12788d3060be6c84905071a5ffafaaecb15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 Jan 2023 16:34:24 GMT
ADD file:295faaf493f6a8d3e2a3eecb28c8f5ac765a1281656221d0a3ab482312a5ee28 in / 
# Wed, 11 Jan 2023 16:34:29 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 02:33:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 Jan 2023 02:34:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 02:34:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 Jan 2023 02:35:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 Jan 2023 02:35:49 GMT
VOLUME [/spiped]
# Thu, 12 Jan 2023 02:35:52 GMT
WORKDIR /spiped
# Thu, 12 Jan 2023 02:35:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 Jan 2023 02:35:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Jan 2023 02:35:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9d653aeb7081a0b221d1160bd67b030696ca49b7ca91912bf298835f8f75ac7b`  
		Last Modified: Wed, 11 Jan 2023 16:43:17 GMT  
		Size: 29.6 MB (29619870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abe6f03d096edad9cefbcccc088c938e23a7055d4351e8cfeb37aa5787fb436`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f896ed2d956a527e2710b5814c6c336e0ced9a98209fcd3432f2dd10b6b67`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d27e290b4bfbefbe11ef090278d14200ce78aae72f617a0c45b72196694ec6`  
		Last Modified: Thu, 12 Jan 2023 02:36:28 GMT  
		Size: 5.7 MB (5705001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95502918743e976e174ed1430de13433c908c65971251adc0941ed528de608f3`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ec717daf1fdf53be4cb1236d04557051ce2dbbf0239b4bbe63b835eb3dd9af`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:30875847cb61b6e1e9f3b5ef6700a0d0eaeee0fdbe93d9844aadf8e286f45472
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41271646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e663c415cbc813e4455e17f82e9126ad10b3ce41a1a913f8e3c7c4bedff18979`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:15:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 17:15:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:15:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 17:16:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:16:05 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 17:16:05 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 17:16:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:16:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:16:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfbdb5fc624191d3f46fae3517ddc1d9e13099a128f28c9c072bc90ec1544dc`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778da259d3954937b144a1302513548989f72feacb6e03870d9ac49002541911`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78952c4b6fad0cc7a3dc3cc41e933cd84346f3b54fe8ec183e7316c0b7087bb9`  
		Last Modified: Sat, 04 Feb 2023 17:16:44 GMT  
		Size: 6.0 MB (5999596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0908ade9b64212309ad3d33772064d6b1be92c2cd3a30c09886eb718fdfec250`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeec2b6d00157ae684bb6c4a1d08d28bf4a0a98c5ee968e5d85e7af5f0ec930`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:ce90d8c9c4121874af31c7fb7f2b625d61671dd1a95ce7c32e652d202cbb546b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34820311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91ddadcd9b85198af8fd4ceb73151e93cb79de37b0a5b31d7259deb2d70116c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:15 GMT
ADD file:29a3ecb38611dbbb6f45b2d10ad3cee60c0198429376f999e9a397f9c405820e in / 
# Sat, 04 Feb 2023 04:06:17 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 08:49:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 08:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:49:18 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 08:49:18 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 08:49:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:49:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c6fe4d1ef15da79055e0a71952e1a38f799d4f36e9acebdb1ec1512651b39f1`  
		Last Modified: Sat, 04 Feb 2023 04:10:27 GMT  
		Size: 29.6 MB (29629678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dc1bc8bba5799858fb508b0c9f5a42fea7a6c0c9eb8de3b35db1d973fc6d9e`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0706fd31877fe4e89e6f262040926d1ba14e7b7fa79f0dcae19ae4e31f3f`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32c2abc910e11be92a564001147caa29ce390b91f354136cbbfb5203c31d0a9`  
		Last Modified: Sat, 04 Feb 2023 08:49:49 GMT  
		Size: 5.2 MB (5187378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6169f704622be973593aff410bf27a3c9ec307c98ded94cd405c8a6c2e09e7`  
		Last Modified: Sat, 04 Feb 2023 08:49:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04839df6cf6945726323210131a6af490b1cec7f3a2d959e8cd96d95dc9bd0b7`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:e8982ce4c33ed5c5fdf992ccf6c890b82d7806e41d8778ea6777610d0e4e4719
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
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5a87be0c5f3e288adf33abd9c67087730cd729e12ac28ae4b107955683edff20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63961a94a731d4f9e0005f5fd83043126c5546496fa856ea125a5c2e51c6979c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:32:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:32:52 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:32:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:33:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:33:02 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:33:03 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:33:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:33:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f659d5259c21b4ce33d18c83c0251b9d66d58281847f63904bed75a5683b3fde`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decaf35186276ee535aac72c69938baded768609a2bb148ca4d5c0a1788a984`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.2 MB (1221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93194a8cc16c2fcd24da284630284cd3fbf877fc323c8dc65e3d256d777ac04a`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 208.6 KB (208637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02decf839b354e56295448b1f40e50f813a1879598a091e766908a8f70b21671`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2035a6bfb730bee20ac317d153b1061a4002ce6a450bb74f34bebcfa04369`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:e8982ce4c33ed5c5fdf992ccf6c890b82d7806e41d8778ea6777610d0e4e4719
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
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5a87be0c5f3e288adf33abd9c67087730cd729e12ac28ae4b107955683edff20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63961a94a731d4f9e0005f5fd83043126c5546496fa856ea125a5c2e51c6979c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:32:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:32:52 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:32:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:33:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:33:02 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:33:03 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:33:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:33:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f659d5259c21b4ce33d18c83c0251b9d66d58281847f63904bed75a5683b3fde`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decaf35186276ee535aac72c69938baded768609a2bb148ca4d5c0a1788a984`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.2 MB (1221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93194a8cc16c2fcd24da284630284cd3fbf877fc323c8dc65e3d256d777ac04a`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 208.6 KB (208637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02decf839b354e56295448b1f40e50f813a1879598a091e766908a8f70b21671`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2035a6bfb730bee20ac317d153b1061a4002ce6a450bb74f34bebcfa04369`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:1d577045d45b0ae89721417ce0ff12570df1a60bdfd748dd9ece51cf4a9ab0bd
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
$ docker pull spiped@sha256:80b3e8ee4628829b3e7808844f5491d7f5a428fdf34b222f015a585458fd6f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37398423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7988b8379fddac2783b6ba47c03be52fd318c7d8a15dc38a46be7959eccd9d24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:35:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 13:35:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 13:35:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 13:35:33 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 13:35:33 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 13:35:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 13:35:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb43ec866fe3cc317a36fa75d6ec2cfaecbf61259805e686134135c2feb7b2b`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b847f081ab25a6a60a0f9227658a9ed04ca809493ef1c23370f819960fae4bf9`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440a618898e824f0daa5b9e12c764cfa879588620c3bee3b56d387ba756975c6`  
		Last Modified: Sat, 04 Feb 2023 13:35:51 GMT  
		Size: 6.0 MB (5998255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395c945c21da9e37967288c6017ab0ba47b905a00c659e8c31051f77c9203ecc`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45038da82a8a6524ba8d5a36b01c7a21b85e45394fa51148b68b43658739b9c7`  
		Last Modified: Sat, 04 Feb 2023 13:35:50 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:883367b70f604d047a082cc4f152f3f4f802288402e3722ce365f1f6c59bad07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33930181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ad7e21ecfa7a20adac9a632da3ad3ad473a297d33eb155fe7d2ed3bff9e682`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:38 GMT
ADD file:ce468627e54d8d1c839cea8ab62e505f612298fd97d50e189293fcfcc6af03a5 in / 
# Sat, 04 Feb 2023 02:46:38 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:01:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 10:01:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:01:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 10:02:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:02:02 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 10:02:03 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 10:02:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 10:02:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:83735a64f458d40820e4310d632e8bb1dc888f6c25114496be3ce431b5f21d5d`  
		Last Modified: Sat, 04 Feb 2023 02:51:43 GMT  
		Size: 28.9 MB (28898637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bdfb7b24b8646ef452836b9abcc4c73c0b7f55202ffa710d2bfaa65bc3aa1`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326bd6c277911d1d0cfa04ad295df1221e1fa32219c63d53f206cff44c355972`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511f46b32e187e216348661375893cbc04fdb397813ccba4bdc9679db4824720`  
		Last Modified: Sat, 04 Feb 2023 10:02:21 GMT  
		Size: 5.0 MB (5028361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52724ebfc8187d2778a989c84f0be4e017eea25ad3ef2cff5d818452ba97cee3`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1834f6fe2aa9fd01acc280547a4ed704342f7ac354b6d8c407911380a787dff0`  
		Last Modified: Sat, 04 Feb 2023 10:02:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:ff2d37d643dba46ec1ca3f190136140c2039c88ce18c8c3c1cda35f75841cd7b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa13aea4e448660a02807e09e9f129b075ddcd15f4f5207e4a1d5c5ebfa02de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:17:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 21:17:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:17:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 21:18:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 21:18:16 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 21:18:16 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 21:18:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:18:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 21:18:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343813fba016b62cf17ebead34dba4d1126a460796db3fb269bebbd3fe2cdd01`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45570ed34e4ad5a6ea26a074f5aac8422e806304219c4b46a060487b4f28b5`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f648b1f6094ef5bd0966d575b58cc91b17e6313884799f5d38b8d591562127a`  
		Last Modified: Sat, 04 Feb 2023 21:18:54 GMT  
		Size: 4.7 MB (4748967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8963d89184feb68cbf98f295746b3544bbd9caa800dd9e59f2a8e7bff44cc1d`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959a250310debb236e8572275069607e0465c91d2c1db38ea09bfc4176dcbe42`  
		Last Modified: Sat, 04 Feb 2023 21:18:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:e99ea9f84c5e7227931a654635c48c2412677415cf41f22e9cfaf34891c29ff7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35320612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0306e8774f16019968e446127b379b0d1696e2cac8d17b7e0168198cdb22e2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:45:22 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 17:45:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:45:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 17:45:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:45:42 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 17:45:42 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 17:45:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:45:42 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e0bfebbe73df67f67a93f5cbb234e1280ccce0f38bd5afa6d69af18cc7cacd`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943241ea7d66696ea790525f04d919838ab68408d32c67ef6e6a1d87f0808b02`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60dfd4f224ba8c244ec6b8489cfada1dff311fab9c3de9c10335d009e99c637d`  
		Last Modified: Sat, 04 Feb 2023 17:45:58 GMT  
		Size: 5.3 MB (5272564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4ddd6c193d40bfbdafb184d07f66eeecd27589a446d6d4e2b33d3e3533a53`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a476866dbd7db5b6a17bcfd9b21f41336bd255c7feb0bee8a8445df77a2c2033`  
		Last Modified: Sat, 04 Feb 2023 17:45:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:3b5039822964df0400c1c464337e7eb24a76e514762eecf8266356c255a8bc20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40269264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9365baff0a3fb27f1f66b81d2a56556b6bd2c28306db3172f2c38d67541c62a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:37:03 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 21:37:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 21:37:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 21:37:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 21:37:29 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 21:37:30 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 21:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:37:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 21:37:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283c04967521e536e9cf08d98eb23ae5ad68d198149c30398cde479eb3fab5e9`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af281af24ba85838614da7407d24c208b44b74cff7983143ad92830dad38133`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf2fb585912d154cc8f37a974f45e7282c72ab0ddd491c0f49bb3fd8acfe30`  
		Last Modified: Sat, 04 Feb 2023 21:38:02 GMT  
		Size: 7.9 MB (7890521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1d975756e334c454f6b84b9a3dc6fbc07f5917a15e139408a47515bd364d79`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5442e2600347208e73136ad766df54a7c9fdfeb85ebaabc9c55fa6dd3dbeaecd`  
		Last Modified: Sat, 04 Feb 2023 21:38:01 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:b730466434599fad0c0b7f45842928f46d35b73a8aeaface9fb6ec3b163a8942
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7df08512320dac74f33c923af82d12788d3060be6c84905071a5ffafaaecb15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 Jan 2023 16:34:24 GMT
ADD file:295faaf493f6a8d3e2a3eecb28c8f5ac765a1281656221d0a3ab482312a5ee28 in / 
# Wed, 11 Jan 2023 16:34:29 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 02:33:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 Jan 2023 02:34:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 02:34:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 Jan 2023 02:35:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 Jan 2023 02:35:49 GMT
VOLUME [/spiped]
# Thu, 12 Jan 2023 02:35:52 GMT
WORKDIR /spiped
# Thu, 12 Jan 2023 02:35:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 Jan 2023 02:35:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Jan 2023 02:35:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9d653aeb7081a0b221d1160bd67b030696ca49b7ca91912bf298835f8f75ac7b`  
		Last Modified: Wed, 11 Jan 2023 16:43:17 GMT  
		Size: 29.6 MB (29619870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abe6f03d096edad9cefbcccc088c938e23a7055d4351e8cfeb37aa5787fb436`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f896ed2d956a527e2710b5814c6c336e0ced9a98209fcd3432f2dd10b6b67`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d27e290b4bfbefbe11ef090278d14200ce78aae72f617a0c45b72196694ec6`  
		Last Modified: Thu, 12 Jan 2023 02:36:28 GMT  
		Size: 5.7 MB (5705001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95502918743e976e174ed1430de13433c908c65971251adc0941ed528de608f3`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ec717daf1fdf53be4cb1236d04557051ce2dbbf0239b4bbe63b835eb3dd9af`  
		Last Modified: Thu, 12 Jan 2023 02:36:22 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:30875847cb61b6e1e9f3b5ef6700a0d0eaeee0fdbe93d9844aadf8e286f45472
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41271646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e663c415cbc813e4455e17f82e9126ad10b3ce41a1a913f8e3c7c4bedff18979`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:15:06 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 17:15:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:15:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 17:16:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:16:05 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 17:16:05 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 17:16:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:16:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:16:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfbdb5fc624191d3f46fae3517ddc1d9e13099a128f28c9c072bc90ec1544dc`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778da259d3954937b144a1302513548989f72feacb6e03870d9ac49002541911`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78952c4b6fad0cc7a3dc3cc41e933cd84346f3b54fe8ec183e7316c0b7087bb9`  
		Last Modified: Sat, 04 Feb 2023 17:16:44 GMT  
		Size: 6.0 MB (5999596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0908ade9b64212309ad3d33772064d6b1be92c2cd3a30c09886eb718fdfec250`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeec2b6d00157ae684bb6c4a1d08d28bf4a0a98c5ee968e5d85e7af5f0ec930`  
		Last Modified: Sat, 04 Feb 2023 17:16:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:ce90d8c9c4121874af31c7fb7f2b625d61671dd1a95ce7c32e652d202cbb546b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34820311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91ddadcd9b85198af8fd4ceb73151e93cb79de37b0a5b31d7259deb2d70116c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:15 GMT
ADD file:29a3ecb38611dbbb6f45b2d10ad3cee60c0198429376f999e9a397f9c405820e in / 
# Sat, 04 Feb 2023 04:06:17 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 04 Feb 2023 08:49:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 04 Feb 2023 08:49:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:49:18 GMT
VOLUME [/spiped]
# Sat, 04 Feb 2023 08:49:18 GMT
WORKDIR /spiped
# Sat, 04 Feb 2023 08:49:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:49:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7c6fe4d1ef15da79055e0a71952e1a38f799d4f36e9acebdb1ec1512651b39f1`  
		Last Modified: Sat, 04 Feb 2023 04:10:27 GMT  
		Size: 29.6 MB (29629678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dc1bc8bba5799858fb508b0c9f5a42fea7a6c0c9eb8de3b35db1d973fc6d9e`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94e0706fd31877fe4e89e6f262040926d1ba14e7b7fa79f0dcae19ae4e31f3f`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32c2abc910e11be92a564001147caa29ce390b91f354136cbbfb5203c31d0a9`  
		Last Modified: Sat, 04 Feb 2023 08:49:49 GMT  
		Size: 5.2 MB (5187378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6169f704622be973593aff410bf27a3c9ec307c98ded94cd405c8a6c2e09e7`  
		Last Modified: Sat, 04 Feb 2023 08:49:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04839df6cf6945726323210131a6af490b1cec7f3a2d959e8cd96d95dc9bd0b7`  
		Last Modified: Sat, 04 Feb 2023 08:49:46 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
