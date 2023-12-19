## `debian:trixie-backports`

```console
$ docker pull debian@sha256:17f38727584ebe3bbab2f2d1b36eb3c66824f647190ab7d7c9efcf0123151dca
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

### `debian:trixie-backports` - linux; amd64

```console
$ docker pull debian@sha256:4afe3ddc85050711dd20fe95d6192c143276d0d27c1f39a8460d807516d44bfe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49583648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2331c37115f9f50128560604b9d39e5e3640c6ec1f38752123174ef172be06b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:23:09 GMT
ADD file:29b09152e341e5171aa28f4c4418697f0618e77dc8ad357953cb4e571071f7ef in / 
# Tue, 19 Dec 2023 01:23:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:23:13 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7ff2da0727c582fb559afda4ae37f2ea848c8d7098b1d441c8dd7223abd5ff94`  
		Last Modified: Tue, 19 Dec 2023 01:29:35 GMT  
		Size: 49.6 MB (49583423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66eaf40a995ea24ea47cb1cde20c76f129d3ba2c6bfea7bfb786042f8cc483f`  
		Last Modified: Tue, 19 Dec 2023 01:29:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:7cddc058435702f38a72df7992183b652581c733316fc8caa0f38dcb66d0562b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47284973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7de52309ef1afb6e32e570c1f1da580638acd35cb29cd7679bcd87329f3aa27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:56:48 GMT
ADD file:4525655c4460af6f1eea7b808845971f5115dc53bd3d22e1e5b904174f4a7de3 in / 
# Tue, 19 Dec 2023 01:56:49 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:56:52 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ef1355a3f40d35583d398e1a76163ce9edc9f474167738235259b9821b4cf763`  
		Last Modified: Tue, 19 Dec 2023 02:02:10 GMT  
		Size: 47.3 MB (47284749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c730352c16708aa532bd25813c73e43c143fc322889e006a66abce2407813c53`  
		Last Modified: Tue, 19 Dec 2023 02:02:18 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:95be1e4bb1485d1ce3b418261e85d7e2318009a3dc6acd232b8a9c21d694169d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45080780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9395387b41a445198870e05486f60d1740211e1f28ee5f15c3cdb8e0af206c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:10:03 GMT
ADD file:3a9b07d7d2dd3958b5dd3f5e10d02d2e2f612023edc0a993b72001585b39fffb in / 
# Tue, 19 Dec 2023 02:10:04 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:10:07 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5fdfd0725abb7810a629f5d363de8fc6e2d9dcb7251dbd35de649c96745cd052`  
		Last Modified: Tue, 19 Dec 2023 02:16:07 GMT  
		Size: 45.1 MB (45080555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fae24938243aa5890e8bb62097ea0e44b52afb8d645cc3ef3bb6ae1ae4dd9a`  
		Last Modified: Tue, 19 Dec 2023 02:16:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:736809cdcaf6b4aaa95061f2d20b296649d3824fe2b5a5e29ee2929926e30566
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49615326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c326b07ed970e68bf9bfa4a29143e5a854ebc7a4a2cc77b01a60c33885a59e74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:55 GMT
ADD file:3a7cff48546e976afb3192375ccd816fa228a2a86ca359ad2d25968d89736a30 in / 
# Tue, 19 Dec 2023 01:42:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:42:58 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:54db10be8b28565099ed8931d6e2048335ac2a2e8633f5ee9961d35950099935`  
		Last Modified: Tue, 19 Dec 2023 01:48:52 GMT  
		Size: 49.6 MB (49615103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbcb4c662cf9bb84bf43bfb322f5b4bdf7ec25f6e4d2fd105b31692a870c57a`  
		Last Modified: Tue, 19 Dec 2023 01:49:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; 386

```console
$ docker pull debian@sha256:726aaee8b8d133df57f780dbc6ce53cf9a4623d91ef1a8643d66d86db6fc6875
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50558742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f5fcf4bcd176985c6f0175521081a2435a8c2dc7385eb0cddd3d8c5ace30a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:50 GMT
ADD file:07e1f2376b64d47d8fc403056f0e46229ed95c88b19adf23f6eef7ed32a4efb4 in / 
# Tue, 19 Dec 2023 01:41:51 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:41:54 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:682156734dfed71ff79e9a6ecfa1d4b20e0cf3af70b52b635e877f84f0ed468d`  
		Last Modified: Tue, 19 Dec 2023 01:48:53 GMT  
		Size: 50.6 MB (50558518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ced0113e8cd7e2ac4374261e160f891395581a14212ccd5d9979f956e71e01f`  
		Last Modified: Tue, 19 Dec 2023 01:49:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; mips64le

```console
$ docker pull debian@sha256:c5b6805f553542c2c0740e2146033aa19c4ca0ec6e0b2f1ae1adf5e61e116f35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49068625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a93dad04548e7e27a6add5681a0bd23ef32ae9fbd8cd90d2f003543a2e154e68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:20:17 GMT
ADD file:8ea6310c27e7f62f29291d04a24b83af6da2d5e3faa1996293119c2feddc0c07 in / 
# Tue, 19 Dec 2023 02:20:23 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:20:37 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b33999eae7d9b8d6555148eda58da0cc5207bcf4c08ed630879dc0190791680f`  
		Last Modified: Tue, 19 Dec 2023 02:31:43 GMT  
		Size: 49.1 MB (49068400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4aa94733c79b4182019330dfc1e45742ea33e476018dc969212c8de5e604fd`  
		Last Modified: Tue, 19 Dec 2023 02:31:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:aec884b732eef1974d8c10eee527275076bcf64809f3e1a0525c3b1e0497c130
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53476704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54950a80c952ea38da80641c967581e6289d977294d42fc75c3b7e9c0e1813b6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:24:15 GMT
ADD file:0c76fa40c0d4d6eec23b49588ff6dbe4b5563f6db327a13831ab7eb6e3f30743 in / 
# Tue, 19 Dec 2023 01:24:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:24:22 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9aa21f27abca3b3157546abcfde68519068ba019777333f48885704721c81290`  
		Last Modified: Tue, 19 Dec 2023 01:30:10 GMT  
		Size: 53.5 MB (53476480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3182b5da1746e4fdc7acb84e703e40ceb03fd77fc5bf61a413ba1c284a5db832`  
		Last Modified: Tue, 19 Dec 2023 01:30:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; s390x

```console
$ docker pull debian@sha256:f9a5f3ad766cfcb6b2ca297c061c562a797176688dd83e646741f4235a443167
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49047953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a5974c842b6f2e5f66a4d8dac3b686731d20debe73c23a2402c03dcdf98a5e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:45:30 GMT
ADD file:b16365f9cf7d013b9f58428c1e63b824b4c10cd69e7e4899e47af1a279108581 in / 
# Tue, 19 Dec 2023 01:45:33 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:45:39 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b824578a72fec7523b71b452ffd659ecf374f66d41368945e63eaefb55285ad8`  
		Last Modified: Tue, 19 Dec 2023 01:49:59 GMT  
		Size: 49.0 MB (49047729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba04a60e8636ce00990aa56b5148aa09e1c6f504df862ee0864186d2f3b0917`  
		Last Modified: Tue, 19 Dec 2023 01:50:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
