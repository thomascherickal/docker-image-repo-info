## `debian:stable-backports`

```console
$ docker pull debian@sha256:d5c5c1d539753a3eb8d385604252595ceb1810c3ee21499135b70ce18321ceb8
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
$ docker pull debian@sha256:79714323782de789a9ac7913b0163a9d96ff8939a9a1728aa9150b89317bc6c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54927085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93e0a6862b88c00c2f9530da5c49609e0598b81d9b5d171309f6fc1fea8076a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:09 GMT
ADD file:fdda2f52e9e1dba71f97065d59c10f30c9cc3031e6be6f5e876d53dd101d4311 in / 
# Fri, 03 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:23:14 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a169e871cbe85334d8ec41a9d36ef90ed3a1c9a841cd569f6e69a132b55e534c`  
		Last Modified: Fri, 03 Sep 2021 01:30:57 GMT  
		Size: 54.9 MB (54926861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e54d8746b00911281004e73ac6c59a6f5e717b987f401116ec9082619c8940`  
		Last Modified: Fri, 03 Sep 2021 01:31:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:ab8eb021de8ee6db0898e02836e6bd7ab54a046df84ca0459a7ec9819cb41557
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52461725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea07bf5358a209650f7b364fc9bf39f9f92414012a8583d3dee69ba9b729b2b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:54:26 GMT
ADD file:908314d8fd5f7710447d1b19e37d844fd54e772f66348508300c7c51136c844c in / 
# Fri, 03 Sep 2021 00:54:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:54:38 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ebd0d6a1ae2c3ae3d1e30544506572ee4409f114a220a97f57772bca9d821e1b`  
		Last Modified: Fri, 03 Sep 2021 01:11:58 GMT  
		Size: 52.5 MB (52461501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c624d7c78496818dd5f2414af61a103a3c6315fee196f1d421c76616b75a891`  
		Last Modified: Fri, 03 Sep 2021 01:12:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:0343c944cbb20c21065f7e14e4175623a839f26f6efd21eca21e7bcf67d11e1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50127483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a820cd320091b4651e14036925b4e85d4219ee620305b0a44ec0052784838`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:03:48 GMT
ADD file:7464f26d5013556d325788672457271f1482968e327d19f7343cda0be98447c5 in / 
# Fri, 03 Sep 2021 01:03:49 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:04:01 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d7c64607233a772e86e7c98f2898a771ca7f1cdef55d721a73548ac0b16ff5ab`  
		Last Modified: Fri, 03 Sep 2021 01:20:44 GMT  
		Size: 50.1 MB (50127258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0daf076b2157aabeab3ed9cf411b2f86c1bf13f2deedb16cfbd70b0f3a40d1d6`  
		Last Modified: Fri, 03 Sep 2021 01:20:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:3f19b499dac785c42598e2381f52d81c306930c7607a63ba4091624e7ac5a70a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53613258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96991d725bcd14bf12f5054ab94c037d8a7d1db2ba8aeb9d3f76bb86417bfcb7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:11 GMT
ADD file:5ba2f2fbdce5a6e494877ea34b03b0003037f1040019ec546d45bc6c6c259ed2 in / 
# Fri, 03 Sep 2021 00:42:12 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:42:17 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:97d29e55b1af03f05bcb80939fd51fe54fe0a33107c9b031c8109591de6f4f31`  
		Last Modified: Fri, 03 Sep 2021 00:52:15 GMT  
		Size: 53.6 MB (53613036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae31bf992aed8687b95dc89e12849a94e2d1a755536b8ec1fb5ff25598bb94b`  
		Last Modified: Fri, 03 Sep 2021 00:52:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:2ff260c808e33ee766416f2b8a83da7db1e2dfa88a0a32bd5697452688972713
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55931151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f609af21bebc9c462e4e8ef37c95847792750d3ba16102b32a493fd3eccc2673`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:01 GMT
ADD file:945b61ddbdb17b71c5d2b3f8cefebbae6b7d28a1723e8a996b1bb23e8dee91ef in / 
# Fri, 03 Sep 2021 00:42:02 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:42:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7a468bfd6e40f25edbf9ee0c8c3160fdb68f80328c8ff2d25c5318e33bacc148`  
		Last Modified: Fri, 03 Sep 2021 00:52:01 GMT  
		Size: 55.9 MB (55930931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3d916672b9b06004832e450bcc69278674f7081e441a6b7add938dd52c53d9`  
		Last Modified: Fri, 03 Sep 2021 00:52:16 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:92b1ab03a3b185c265d9cab385edb64b63fba9825c658530024e3d017436d961
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53177406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23714c3e898bf9dc1e75f1c381f7bf7e05ff6cdc41adbf4fc4374ef8621a7e27`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:48 GMT
ADD file:027eda15910b8858f29e73fae2027996c266ea9b1fbb74e7e3702421edae5396 in / 
# Fri, 03 Sep 2021 01:12:49 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:def7717bcc5e494128c1aba2c8eaf9f5826d8b1a92ac1fde020434f2edc3ac34`  
		Last Modified: Fri, 03 Sep 2021 01:23:05 GMT  
		Size: 53.2 MB (53177182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eaadc85450c3fa2b5403303675078a868d6cd840cde8823a9f472e56ff10754`  
		Last Modified: Fri, 03 Sep 2021 01:23:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:c31ded44cb3bbffcafbcde92fa425e33363648bef803e19ae025d6215d3d4016
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58819650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0b25087a8ab592dbc57cac7a0fb2ede7387e440f306bfb9da070ac099bc8c6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:59 GMT
ADD file:65fd9862530d73959aa4b1a794c58ad4fd4fef5e64c3a5a48386cbc75b5a1b77 in / 
# Fri, 03 Sep 2021 01:27:08 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:27:24 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a8d6f167deff8b537d96bc08a0664b47da9250cf4f4f5f2726008df2ce0db1be`  
		Last Modified: Fri, 03 Sep 2021 01:44:46 GMT  
		Size: 58.8 MB (58819425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d20444ab3a29a7f981bcdaf28c31848b34b558259b0423e3f31680a56b50615`  
		Last Modified: Fri, 03 Sep 2021 01:44:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:84e37e460f3e8d662a44c40afe7862fbf92f1d32f957f4baff5e47027c32cec9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53201380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa73ba6de831402b7bcada29a1da0b63331d5984e125e84a091c05ef2502fd92`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:50 GMT
ADD file:36fd9ac0c89a5ce05424214a6f58fde9af80187b8f71917173d2d8db397cc903 in / 
# Fri, 03 Sep 2021 00:46:59 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:47:09 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0da7bc376ce3e71bc09bac21534e8dbcc899c6b4058ce5faf9ec32cc07224cbf`  
		Last Modified: Fri, 03 Sep 2021 00:55:01 GMT  
		Size: 53.2 MB (53201158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832979933e4d7cc1aecd547451f444b7ac3886ebc4ab1dceea21a3eea5c21e87`  
		Last Modified: Fri, 03 Sep 2021 00:55:12 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
