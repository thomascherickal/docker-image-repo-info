## `debian:experimental-20230919`

```console
$ docker pull debian@sha256:c591284ee1680f4ff8e9a73103fd6e549ded0de0c5c1312d27ec3a6ff0417b52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v5
	-	linux; 386
	-	linux; riscv64

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
