## `debian:experimental-20230919`

```console
$ docker pull debian@sha256:c5e0f36444d1308838ca5e1ef77a301b5a45a694de84cce509e98f628d0799d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental-20230919` - linux; arm variant v5

```console
$ docker pull debian@sha256:238c202e5e07122d00f19c305fb64f11a1bb4fef6c5d3a1a89488b7050a8f98b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47166110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fff5d12d0cf3723b278c28a516acffa97a5c604936bd81e7c829fbc500c4890`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:52:49 GMT
ADD file:efacb4b54656a7d70efa5581608c5107764d5c325ef3525f20da886cc9d2db15 in / 
# Wed, 20 Sep 2023 00:52:50 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:53:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3ea5112c05eb52a1a7adc2e1ff947d9ef11dd65aa8db61d85f145977de37d94b`  
		Last Modified: Wed, 20 Sep 2023 00:59:38 GMT  
		Size: 47.2 MB (47165888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fa3e57da9074002184c9ddd5e1b6b880d33e866055f1ff4e8bf97f1ed879b6`  
		Last Modified: Wed, 20 Sep 2023 01:00:06 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230919` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:538261bf0e9adabdef459fc5866ddf8ed62376fd3d93bd826f367d0bb2359467
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49450712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21941270492380aa35b48a746947e8290371565abbac1132b0f9d9e100019abe`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:46:12 GMT
ADD file:c490dc1dd969e985b6ee09de2811426fe3e1f59c999434c58165f20e12999c58 in / 
# Wed, 20 Sep 2023 02:46:13 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:46:21 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3c7710302475abe138bbc1da10c4dd6cf01afcbcc1832cd54e1f313291e8304f`  
		Last Modified: Wed, 20 Sep 2023 02:52:00 GMT  
		Size: 49.5 MB (49450491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1cdcbc9d4070abff87713c27d593a64d42b3322b78f0b6af668886085ae7e9`  
		Last Modified: Wed, 20 Sep 2023 02:52:19 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230919` - linux; 386

```console
$ docker pull debian@sha256:2586381086b7ba3f454eecd770fa8b24c681d0dabdd14f9b4277085a9b7a30cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50483356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58bd669e2db5cc1fb364d2b8e3e5bd6f318c0da3770d12b366481fcd8de0f9b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:45:00 GMT
ADD file:3bb4d051fa5479e355b15385abeadbfa837f0821c7bb7deae4ef60cdf97a818c in / 
# Wed, 20 Sep 2023 00:45:00 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:45:12 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:68e4fd76cb5525e54a59b89c74b172e28043f1983c094aad05f784f90f3b67d6`  
		Last Modified: Wed, 20 Sep 2023 00:52:37 GMT  
		Size: 50.5 MB (50483132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a9afcc3ec989f19fd54d38ea92d23b13f7eb0a710358015dde31ed56a53cb6`  
		Last Modified: Wed, 20 Sep 2023 00:53:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230919` - linux; riscv64

```console
$ docker pull debian@sha256:e08fca1312c295ab8ad2841f4ed6e36de03309c233d3051874170ab4a7ae03f1
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47886230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc784227faae7baba952fabcb31d5132bea3cc613402980652031e499def33dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 01:11:45 GMT
ADD file:6a9fad96e58d832f0ec36c085b5b9904ae84876ad08531f6c3c132d3be73dd3d in / 
# Wed, 20 Sep 2023 01:11:47 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 01:12:21 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b0c261248d3418f436857a29cba81500d32de6cb99f0dec9332afcf0a92999f4`  
		Last Modified: Wed, 20 Sep 2023 01:14:55 GMT  
		Size: 47.9 MB (47886007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10557eba7c5e511a82e3ea746d3521945b345f619939bed42516bdd75805b5b`  
		Last Modified: Wed, 20 Sep 2023 01:15:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230919` - linux; s390x

```console
$ docker pull debian@sha256:5a99307322dedf61115c8c61178cc6aa594172975bc98e49a799f392a742ca18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48852900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02fe7e50e2d16b207074410719fe24ee58c44062988b89d52f014ccc229d1475`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:57:55 GMT
ADD file:e9daaf010354274abd7155c817f9f0c0889b2b3fe50962a29228c1a581e324d8 in / 
# Wed, 20 Sep 2023 02:58:00 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:58:16 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e1754847300a3ceac393bd835ca20897f0a02ddba5fbcd6885ff3d590022adc7`  
		Last Modified: Wed, 20 Sep 2023 03:02:44 GMT  
		Size: 48.9 MB (48852681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfb653229f1a934cc13e5a0e8fd136a5e3b0e0b4fb3a0a36855660a8de28edd`  
		Last Modified: Wed, 20 Sep 2023 03:02:58 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
