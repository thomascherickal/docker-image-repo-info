## `debian:rc-buggy`

```console
$ docker pull debian@sha256:38849febebbabc0905046195f70b812f3b8d917a01c47b12e2983298d84f281b
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
$ docker pull debian@sha256:9d3610c0e2306e6876512720d8ebb62e6b8919a043e9e7fe7521060c39924348
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53226575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:190655a4f2734190d775752554eed721d56915fc036a331364c69747c464624b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:07 GMT
ADD file:0aaeb8a0c7fde9f030dc2ab67a03f21f44e9eecad9e4cf1f360dc5f768292460 in / 
# Tue, 12 Jul 2022 01:21:07 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:22:30 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4a81bc091a3ce5ccc3c89ef56e710ee1854c5ff9fd3d7f148e87cb956b5b78c7`  
		Last Modified: Tue, 12 Jul 2022 01:26:19 GMT  
		Size: 53.2 MB (53226349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91330c622ce4660eadca8299d6e9ab74e7e6d0349bbe8669a2e92011a0802a2`  
		Last Modified: Tue, 12 Jul 2022 01:28:37 GMT  
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
$ docker pull debian@sha256:dad27508fddd14b31239f713bea9907473e3e6c3a92c266cee20ad38968b9a3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52346424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9441e437e2de3f9ba926e0c6aa96685495517acb3f82accf832ab5095363bf62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:44:00 GMT
ADD file:f6825f1dd59126d26ef0dba330a1d0eff37f6b9d56fe4a1bf2669774a6a7c74b in / 
# Tue, 12 Jul 2022 04:44:06 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:48:29 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:043042ab5eb51d2e5fe9f7bf85b86a91823ebf404e02b09bd9d96e29066acc7b`  
		Last Modified: Tue, 12 Jul 2022 04:54:59 GMT  
		Size: 52.3 MB (52346196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a5e9a95611895b5cabfd0cade30f902d57be362b69dffe38ad573505508162`  
		Last Modified: Tue, 12 Jul 2022 04:59:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:b10d9485c59afb76be161afc9589cb66f9b5c14ba273085a3302d24925289bd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57441690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d516910cff7c8beb42da0d8e97753f4a37ad2512406811b1565037e2d853b98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:27:28 GMT
ADD file:8039654bddce2cd83d9433d1df0a53c329e7877cc8210593bcde23de63e2f1fd in / 
# Tue, 12 Jul 2022 01:27:36 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:31:02 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0d4394941206b4f218ffa2a2b794698da5149ab7a22b52f71390aec65a7add3e`  
		Last Modified: Tue, 12 Jul 2022 01:40:47 GMT  
		Size: 57.4 MB (57441462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0fc21912991d1e9e72c0624ce9ee5176590907057c576cb5f6e368033ddc9e`  
		Last Modified: Tue, 12 Jul 2022 01:46:24 GMT  
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
