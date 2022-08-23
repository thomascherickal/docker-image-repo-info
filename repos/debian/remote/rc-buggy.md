## `debian:rc-buggy`

```console
$ docker pull debian@sha256:d3636ffc22e072acbe08dffb339039899193a05640faa0bc6c0969e4ab558ee2
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:9992d67868dfab253bbf5653394a705ff0e28a6e96ad664000a48aeb43e0fefa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52769010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe3bfd306ef82aac19d7e07a57e0070b34fbf2f46891b9f5e079fb28007344e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:22:50 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c4d30b5308bd3334b2b5c05480e9c4d59fec4b5ff7b0fe9d08a943ce8a81c0`  
		Last Modified: Tue, 23 Aug 2022 00:28:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:40a39bfb20a5326b54cedd07599e4178e233d187ab83ad1f337877396e1c7de1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52021601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a9fdd2c7b9a24ac8258ba4d765afddba436eae0e18aaa40fa0012143a37390`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:50:23 GMT
ADD file:2829a8dbc1e67454e67c0015efaaceadaa4b04330ed9e60cc8248246cac2aae2 in / 
# Tue, 02 Aug 2022 00:50:23 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:52:13 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:11a67d4cf31e6e9dc8797a5c01d3198f326d91410c372d1a490bf5592578d9b1`  
		Last Modified: Tue, 02 Aug 2022 00:58:37 GMT  
		Size: 52.0 MB (52021372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18be018a4cd1bf36056645404fff6307f19ee97d20e3496d5f8dceafbc5ede39`  
		Last Modified: Tue, 02 Aug 2022 01:02:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:5156950226035fa49a928441c7a39794c177f11e8daf48e17728082e7d0032de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49735578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6cd2bec8c8c6bbc582f899bb7ec91d53c546f043eb7683f3660794600837264`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:00:45 GMT
ADD file:a1d27fd37cd41b3026c10df50adfd5a93a40194548a87a372c97149f63b096b3 in / 
# Tue, 02 Aug 2022 01:00:46 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:02:47 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:23e34b183a37464e321571d2a75fa33fded0e5a8506066db5c4f20153a665c2c`  
		Last Modified: Tue, 02 Aug 2022 01:09:03 GMT  
		Size: 49.7 MB (49735351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d963dacd1cafd3020eaa0e9ba6704250f64b1786dda2a5b6f93abd23c84ae4ed`  
		Last Modified: Tue, 02 Aug 2022 01:11:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:395541901562547336ba97e072140519bbdcd91e2248d601e85e7c29b3d287ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53312011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e83a7bb271ca67ffefac1408baebe65a15152fece45af55b9d896612c2ca5c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:477966410dd9e274b01740d7af857db5c024b4c4e53a5e83b5da6854d5b0c209 in / 
# Tue, 02 Aug 2022 00:41:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:43:05 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:17bcb8e39c7f35480d4c2e5b46b6c0a58dac180206453cc49052707aa8053632`  
		Last Modified: Tue, 02 Aug 2022 00:48:00 GMT  
		Size: 53.3 MB (53311787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181d200df989fe255ecec6ade5a368d9c42e166918167d88567406b9553232e6`  
		Last Modified: Tue, 02 Aug 2022 00:51:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:1a6970d52ecdd4cdfbd99d9e274586a2d4400a3fb9f9853df613ab49b38e90b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54195291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34badd7dd66d1ba04344b377040efe752f22f5681408103c1f7c9e5b2c1f4512`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:23 GMT
ADD file:40a2042e14b22d803da216af628cd6e8603c923c4fe79ca3c4c79c95c1c1e878 in / 
# Tue, 02 Aug 2022 00:40:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:41:55 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ef86b631f45587b4b6d1c16b80732997a4895ae8df072b14d68c25aeff8b901e`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 54.2 MB (54195066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42dd8937bc99798cb21296d166dadf51043660706e7e529aa5eb940eadb98b5`  
		Last Modified: Tue, 02 Aug 2022 00:50:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:9696d90fae16cf745e90e9969280aafe3815fc7e4bf5b6969aad058462bf566a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53216859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea1f44a513ec588c37eafb3901eefb497af60fa63fe64d74e8948e5c424ed00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:16:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ddf2d67b6addc7804c51ac4e7b7d0e5ba53c3f5e82c8de6043acd4b789f339`  
		Last Modified: Tue, 23 Aug 2022 00:24:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:38486e035651cbde5bb8cd523f4c29c3e808cd95d98bd5cdf8d11d5e512c3394
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57440455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a815a76fb94cbf344dcd4e5334ffd04fa8805d950603955b46bdc108c86f3d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:52 GMT
ADD file:6911368d0ae9ca029c373628ddb642f29cabf3f909e9a77f8931355843b8ea49 in / 
# Tue, 02 Aug 2022 01:18:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:20:56 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4a386a4ce4974e6c6fc3a96c6a7a96ce47fa8df11122fa0a4b856c23c5ccb46b`  
		Last Modified: Tue, 02 Aug 2022 01:27:09 GMT  
		Size: 57.4 MB (57440227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7c235d69bb3eb6dbd707ca0e5dc87155b7bb8b4c94c707bb008425cb64f07f`  
		Last Modified: Tue, 02 Aug 2022 01:30:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:a93ac8dab3d5d92fb8b82b7a21d8f6bc8e6acc7d681ffabc19bb4f986c186991
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51734894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c80fcf8432cefd3819197fca276eed0a2db1314b83a65eb088efc34f3dac8cff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:43:36 GMT
ADD file:19dee33de85aac92620de3bd92768833a889db0b60b7445419bccb4285c46f94 in / 
# Tue, 02 Aug 2022 00:43:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:45:19 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:31888e988211ae2cd4058438d0fd3d3420a26d35f21e97741527c1e85ad2d476`  
		Last Modified: Tue, 02 Aug 2022 00:49:29 GMT  
		Size: 51.7 MB (51734666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecdbc978b2d44472a444509cb3623ef651225f637883af28f18348bee92c04a`  
		Last Modified: Tue, 02 Aug 2022 00:51:42 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
