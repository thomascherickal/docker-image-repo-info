## `debian:stable-backports`

```console
$ docker pull debian@sha256:5d0a71e5fb3a8cfc330e495cd55a3b06e01a885b8c5779b694032ab843f99f45
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:07f7459c4bc7cadbe003ab895f8e62b1de34ca49e6b258474d7214f21a0ec556
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54917356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34812039e025404ac7021aec3d9dd6e5dae0d472c9ab5663d31e661edd52714d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:19 GMT
ADD file:521bc1c567092e76fb130d456b9c11bfa41c2b3cabe210ec779f8c11f0b514ea in / 
# Wed, 26 Jan 2022 01:42:20 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:42:25 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:282deafaaa63acc630a61a473bccb94b56456064eb2695532b1cd688f05d2cab`  
		Last Modified: Wed, 26 Jan 2022 01:49:50 GMT  
		Size: 54.9 MB (54917134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7942a9ddcc9a30e13d657d6a39e62e6dd9e2e28de6822ba3b62b4cf65ed85639`  
		Last Modified: Wed, 26 Jan 2022 01:50:01 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:26cbf78b9c9e81444333e782b4c36f838d8857dc5f4d86f7ebb13b57b27df67a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52466832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a7d9206c56c23d80560f73eb201849ec439988b8eca8306aa157b03d122a8a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:08 GMT
ADD file:bea095251461ecef269e26907f39d9dfbf42923f8aabdd2826a1323d6111f6a6 in / 
# Wed, 26 Jan 2022 01:46:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:46:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c5e17197e13971802f8b71d7d93cc867f59ea37a3b5b16bc89dec5524b24cc4c`  
		Last Modified: Wed, 26 Jan 2022 02:03:58 GMT  
		Size: 52.5 MB (52466607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca24351ce40933dfa7781b852fc9d252f402bca57797ca57f35ed9decdd493d`  
		Last Modified: Wed, 26 Jan 2022 02:04:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:83e9201a4961fc7ea753ddee6f3259684810f2b16c4427e8bebce77c913947d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50117619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cc100df5aa5ddad502876ac7f16fb0b76767f503220250b1a6509c0d1098996`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:33 GMT
ADD file:6c3f0ee1e481cc7257b7c2d718fd93960c2671db6bc54b5a66b78de112aac9a4 in / 
# Wed, 26 Jan 2022 01:46:34 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:46:47 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:62631d28c5ef15b979b2783ef7074a87e04c3ef92a8c299623192faa1f3ad6af`  
		Last Modified: Wed, 26 Jan 2022 02:04:05 GMT  
		Size: 50.1 MB (50117394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318f6555a245b29ebcdd3405e0d6d882572f2d6f03ce27b92636d94f00c5e03f`  
		Last Modified: Wed, 26 Jan 2022 02:04:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:752572a05b8a2cde0dbbb42a6cd6fd721828ffce4ee46ed9ea88ccfd560b698c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53609035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f52bd0ce51159c9b59c2a67bddf19e7ab04e751bfa17a4022e7c9deb25b0819`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:10 GMT
ADD file:f526a75a0d394c1d107a60b1d8ef552359f49654933a937cee97e23ef10c3baf in / 
# Wed, 26 Jan 2022 01:44:11 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:44:17 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1c051b547b5970e9ccdf2b3a23cc75ea19737bdf52a04291d45360996f79dc66`  
		Last Modified: Wed, 26 Jan 2022 01:52:12 GMT  
		Size: 53.6 MB (53608812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800adbcbe9b6e8e44c05a62cd7a0b2e4b55e02dbc5677cdca407de584a98407c`  
		Last Modified: Wed, 26 Jan 2022 01:52:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:76b0a5d331838b2346875d7abe968de98c9b8e1ac6ca00b0d0cc3f499ff784f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55939211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28f2667a31c9317fa16a315f306abebd590e9208b2cd7e7f690d0927b7c6c988`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:20 GMT
ADD file:2dc049fc644b450f7708e6ba08cb967f08edc479ba044fc8fd8d13da284f64dd in / 
# Wed, 26 Jan 2022 01:42:20 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:42:27 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7b7daced8c309ed1301cc4e93c8625ad268569c74ada9bfa08006a89cf773163`  
		Last Modified: Wed, 26 Jan 2022 01:53:07 GMT  
		Size: 55.9 MB (55938985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be93cd9a820fa831e5844cb1a1ba948c49e15bc0fb3f725442c3a3c34978868`  
		Last Modified: Wed, 26 Jan 2022 01:53:18 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:2892acf4e6a97bb2748bac120fec16bd5bc4f009ed2cbef844eea21e7542a7ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53180251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb74350fc82c15217c2f935a583b31b97a1e06edf30164aa6ad5a01e6d00ce3c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:47 GMT
ADD file:555d41e6255ac2c7392e7749e39448f6948fcaf834cbf88f3173be7c8275c047 in / 
# Wed, 26 Jan 2022 01:45:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:45:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1a4422bd2d6df0fd77791fd0fc029636b0836449febec22532dfca5b616d530c`  
		Last Modified: Wed, 26 Jan 2022 01:55:58 GMT  
		Size: 53.2 MB (53180026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9917646d4deeb963206118602958bb1116e30cd58f3ffe1306d6cb5ce2dce21`  
		Last Modified: Wed, 26 Jan 2022 01:56:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:dbf758b3b4d84d428d9f6853249ad471601c46ed74ac5024f5ce402d6325e50f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58833750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6793ea9b3d04c8efb492e92c7725548be3c356b76c79188b7be57777682af83d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:49:31 GMT
ADD file:d32062727947876c4866d3ad67a89a969e45a67a63ead3840fce386947b64d08 in / 
# Wed, 26 Jan 2022 01:49:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:49:51 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:66b17c8c79d695b0ef403adf25bcd3f47010408125c5bff6b5ffec652538ef18`  
		Last Modified: Wed, 26 Jan 2022 02:03:08 GMT  
		Size: 58.8 MB (58833527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce51d672cd20b81558d97b3a42f637c863ce974df3a8f48c574c0c6d117b7a99`  
		Last Modified: Wed, 26 Jan 2022 02:03:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:f78e40df1798e43ce2cc7b4e6a48e098da2c5209e5307912a8ee9031bd844b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53210630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96ef3437539651cfcae41f4d15836f13c1f8d18977c5f989a40db016b3270fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:9c461f978ac846a3ad5cb38158e643e891e43a55f6814570368c52ef18c18ece in / 
# Wed, 26 Jan 2022 01:42:47 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:42:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6a3da0087beaf13ce10489cfc2f64df5fd0176e3d0dbd8de86561bb82f750d96`  
		Last Modified: Wed, 26 Jan 2022 01:48:55 GMT  
		Size: 53.2 MB (53210406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cec4fcc67945f51b905cbefef6e43f1ebf38990537b0e8f1274446b3d3bfeac`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
