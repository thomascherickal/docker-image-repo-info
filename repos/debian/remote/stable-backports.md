## `debian:stable-backports`

```console
$ docker pull debian@sha256:9be0dce47da0c0fb3afcb3dd4b530a3a1131e9b089634feb760c05a043a37192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull debian@sha256:1b69562b0845b92ea833164a4fbaebc83d3a018c678929eee925459e2779be4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50396137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45461ef2f1d2a85020d909dd442971e02ea3fdee94409a3b96a5f4dcdf277289`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:43:15 GMT
ADD file:f2331c69596aeb6ba28e1e270ecc5949cad054ad3d77be946661b0b8528c1a3e in / 
# Tue, 13 Oct 2020 01:43:15 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:43:22 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2c81564eab1e9c41e06d27314dfcd84d4c493e4abfc90947224fd4418ebeaa56`  
		Last Modified: Tue, 13 Oct 2020 01:50:22 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debd22ac359dafd85b08bff7077d62b7047d58417816abd4f2934ef5197b5f8c`  
		Last Modified: Tue, 13 Oct 2020 01:50:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:e016e6cea96bc720cd5a7b084c0e13945b1d2a6daa594b8b9760724154af07db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48108861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c79de7de8dd16179f9e8669342f1a9abbd2df39fe13a6eb0d00b229ce9799c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:56:16 GMT
ADD file:aea97b81b51c5ff1ffba73e1adb5edd229a85340a737d8f4ae771a4e7ae3204e in / 
# Tue, 13 Oct 2020 01:56:18 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:56:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c1630d1ee14595a02763aa063896639bd896919f7f8ba199873880709a0dce22`  
		Last Modified: Tue, 13 Oct 2020 02:04:28 GMT  
		Size: 48.1 MB (48108635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286abee35d708db63e21482ebf8727768100acc6388bea5b87c76c750ce337cf`  
		Last Modified: Tue, 13 Oct 2020 02:04:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:828d66565164fc1b808c94da052313ae41ab37d7bbe8f306f9c6c233632d741c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45869501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271b9c8a4b877a054825a7208329c7bb4f2c729b3115f821fa064758bae08898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:03:11 GMT
ADD file:e80347b3fe9a358cbcac1ef9642378d9468193000ac4c7675c3093a6c1246fbe in / 
# Tue, 13 Oct 2020 01:03:13 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:03:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:975a7da0a330d9dc8df9bca417eae2c60f70b757d657d5618e9f740001725ce1`  
		Last Modified: Tue, 13 Oct 2020 01:11:46 GMT  
		Size: 45.9 MB (45869275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15f9d852b973d2943af0a2d575ac34b25c91b6ab67f0252b7221c82dd8ae489`  
		Last Modified: Tue, 13 Oct 2020 01:11:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1fca4cb499e75d74a14a1e22023c9910f9f400e024418d681b63951f1a500ad8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49175603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6ebf3ae5b65b0ad945d274fc39971de3f35c2a5a5044888174bbf504025f582`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:58 GMT
ADD file:5ca7b9d0c7fd89e638c6a9846a2a949742adbcc50cb3800e3feb6c57c368f7a4 in / 
# Tue, 13 Oct 2020 01:43:00 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:43:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c6fb6a7a2dca6918398028c24cd1a0d68872503c88a6e42c5bcf5ba80db42253`  
		Last Modified: Tue, 13 Oct 2020 01:50:04 GMT  
		Size: 49.2 MB (49175379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741f6f3bbd737c6e1dfc4bb74d2b34d67380ffe149d177194704a4e1d2a9e69f`  
		Last Modified: Tue, 13 Oct 2020 01:50:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:b2fb92ebde3ba1d87490753812e97cac6aea5f922942b96130d8f46586f23753
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51158990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dee9d167d8e021389559a72b8e01ddf387ba8e85cf2342ef955b1666f7b808f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:22 GMT
ADD file:e77ee4912c2d0bdacee1491058bca3b4e9146b9f0ebd3062a8daca1b1dfbd0d0 in / 
# Tue, 13 Oct 2020 01:44:23 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:44:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:65d7ff65daaa164da70664c1facda9e3cf1d1a4584d63ca05a804da6e0445219`  
		Last Modified: Tue, 13 Oct 2020 01:51:25 GMT  
		Size: 51.2 MB (51158765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a8cddfa5ee8af2697387481a2977281ed6909293924b09e3b7c89d4277b1b`  
		Last Modified: Tue, 13 Oct 2020 01:51:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3eeb2f48730292b2e2636ba3bf1d58e1d0bce5084fbdd3bbd6890f52c3f8fc93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49017412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d21624baede0abbea429191f7b4cd3d994a0f67103896a1c92c3fe79afff8ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:11:09 GMT
ADD file:72cdfa882f679ce8fa8feeb0c4b3a3c5a11bea9d8274050044345f4c13128c38 in / 
# Tue, 13 Oct 2020 01:11:10 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:11:16 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9335550774ea0cf524a99090bc694ff244784028cd8555713ab381ba13044414`  
		Last Modified: Tue, 13 Oct 2020 01:18:35 GMT  
		Size: 49.0 MB (49017187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd5f6a5dd1c60361d5cd31d2c74f4d66af157fa2d5b2d7c48aeb19dc83bec9b`  
		Last Modified: Tue, 13 Oct 2020 01:18:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:7a69c7c75a30957d2bc280faabad66b2706daf71d02002d0309887e8495f4534
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54142803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca8866212f69ae025270328d78bbce135c28aba0a11ea8815549cb4404bc4906`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:25 GMT
ADD file:29306cc509b6e7b4b2c27509932d4a57cebc93d1a35f875190b20a7ae4eb21cf in / 
# Tue, 13 Oct 2020 01:40:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:40:43 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ad0fee91c0361ab0ded769b6ee3d2333eb0964eec74f3cb8fc5eb2f1a709b9a5`  
		Last Modified: Tue, 13 Oct 2020 01:53:01 GMT  
		Size: 54.1 MB (54142579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e21673670fdb7c234cb9b2c7e872038986b51ca6bef6c685509a066271d9bb`  
		Last Modified: Tue, 13 Oct 2020 01:53:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:4c7cbaecc512ac0580d9938e46f9194c23a2ada48bca45966d793936c9827ce1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48966523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd2ddb629e4c8a13a3b4fac9b447404d3311d7c080c1584a829991c30476b45`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:43:06 GMT
ADD file:28305c36d665c50658295c3a602abc666c49508f0f3f70990069301ca55e0955 in / 
# Tue, 13 Oct 2020 01:43:09 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:43:15 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e23aafa7a2b18d2384e5ffd2a190a16a7836547db442d77848d031e439c9a609`  
		Last Modified: Tue, 13 Oct 2020 01:46:32 GMT  
		Size: 49.0 MB (48966299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687e3217c7c19a9dd87022b667f7f6f2f516ce96f9196d7666c7e2bc104c81de`  
		Last Modified: Tue, 13 Oct 2020 01:46:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
