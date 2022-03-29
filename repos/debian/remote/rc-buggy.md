## `debian:rc-buggy`

```console
$ docker pull debian@sha256:d885d0f9c9fae472c417e5dfc9254b699195ae5dc7af4312021a16d96d6052bc
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
$ docker pull debian@sha256:6dba00554e8e4adebe7f4bc767405597f0d172a3ed9548cb568f5fec953434c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55804626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa1f9338500cdaba5d8d7823713303209fe6318382fc8e924432ecf1348b875`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:23:26 GMT
ADD file:10087b555ac457b6a577fbbc8206355ac696e76dd49ff2a4eeeb27ac8b9f4cec in / 
# Tue, 29 Mar 2022 00:23:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:24:57 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:48f4b65c158eb45a0eb2daaee21a00efa6f1ed6e8943806281db050162c30174`  
		Last Modified: Tue, 29 Mar 2022 00:29:32 GMT  
		Size: 55.8 MB (55804401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23196988c5da0d13b2228875e0a879b26482fee094299347b0717ce3910daab5`  
		Last Modified: Tue, 29 Mar 2022 00:32:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:11dd601e6cf9b92dd2b1b9bd1a3bac7255dbbf6e9087488f5ab62151f83bdfd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53206691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:503b1738ccfed6cfc9ae2e6b9caa241899a4f30f09c4317b4519ec36e0b6f6f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:53:53 GMT
ADD file:8fcd736cc488ae6bc3f8a0a57f5454dbd34b0c05fd62d2bf748eeb34723c2a85 in / 
# Tue, 29 Mar 2022 00:53:53 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:58:18 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:07dd120b73b0ec25351ce0c0743306437c1d81e0ee7e06f053f28a0e58bfa81f`  
		Last Modified: Tue, 29 Mar 2022 01:09:52 GMT  
		Size: 53.2 MB (53206463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49f068b998206c6769e1559923f59236db7f962f81aad7f1a4d1002396a49b3`  
		Last Modified: Tue, 29 Mar 2022 01:15:33 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:eaebc6b06d1c4b3481f15967c6531fc2a23b178e4160b757fcbac1dcbc6b5c6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50813569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:957fbfbd3ad31332b8d8a81193bcf1db2e2f263cad7f6173dd38257f84f649ae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:22:06 GMT
ADD file:c6f82841459351fabc9a42dbd56f6622b4374e2c684eb76537d4f31022fe8774 in / 
# Tue, 29 Mar 2022 02:22:07 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:26:50 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:20059c5e4ca7052150ded6116965ea89f37bd64493315e1aa29821f6adc82ee1`  
		Last Modified: Tue, 29 Mar 2022 02:38:27 GMT  
		Size: 50.8 MB (50813342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc60f13238f0b35f72a3e59e46562e4bc7fe7dc619acb8bb99ebb4f1608b7303`  
		Last Modified: Tue, 29 Mar 2022 02:44:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4137cbd9ae062150e21fb18e9b5f004eec566a2b5095a98ebfc3879e656a4d2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54722282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd98b9f77abb2443712164e42d2236c7e0de0a0e0880604a5cd6081c3a7ef80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:44:39 GMT
ADD file:8299f759b242f8c95152a99fbc389eea6ad6b8b19eea94a657be56f01d578df6 in / 
# Tue, 29 Mar 2022 00:44:40 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:46:32 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:463f3634d113f916cceb251bf5bf6b13c658f1a17397f89d844d16b67f3015f5`  
		Last Modified: Tue, 29 Mar 2022 00:52:40 GMT  
		Size: 54.7 MB (54722054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643a23237d9f25f4accc36375e1af9429985ba462546603aa9d39dd45c12120b`  
		Last Modified: Tue, 29 Mar 2022 00:56:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:8c94f4a4573b40f6e6aada86b8b76ae5ff6455c22160d6836ee0304de91af170
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56838738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07098a914f2561368939d23f9d2aa3af0ab3fb4cc7899c1cd9dcd6a1e0c8da8a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:25 GMT
ADD file:a09b15a232ef12356f8a381e48ebbc75da16b46600e0cc9849189196595b48b3 in / 
# Tue, 29 Mar 2022 00:43:26 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:45:21 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0847c00642d4fc3cd086952d88bb1c62b35fc1592abb8bb98b5f2580cbdf5cc5`  
		Last Modified: Tue, 29 Mar 2022 00:51:53 GMT  
		Size: 56.8 MB (56838514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1909f39ed16ad9f78baad06fd192ab1aee614759874ec48ce0c8f2973d4a37`  
		Last Modified: Tue, 29 Mar 2022 00:55:27 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:4c4cbffc43af22e952b4a4e55f90a68ef2e4241459432ee322a4e879be317f4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54637060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a886c2ea16e3cdb626fda91bd99c00e18f3d14383b532705e5d02a090ba85b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 08:55:47 GMT
ADD file:2015a98f802a1e28eca2c4eba0b574f58c2cd7844c0d94dbf0e29e8180aea210 in / 
# Thu, 17 Mar 2022 08:55:51 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:59:53 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3d194d6caec7e92bc6e1448edd24c61790b7372a62bd6808d5cd0c5a6eda1736`  
		Last Modified: Thu, 17 Mar 2022 10:46:33 GMT  
		Size: 54.6 MB (54636832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f89521f753afea1be4cd913bc183db915b1f5e7413ebad252933b2cd6d5411`  
		Last Modified: Thu, 17 Mar 2022 10:51:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:036d5995f0fe37456f1a835f7f84ec0f3df2d372b88f1b3d556adca4a44b7edd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60217491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662cb550d87bb4bcab693949c91ac75748f26aa5c7ef2b31410beb467d928ade`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:24:04 GMT
ADD file:a3e83f143a1077db22a0c3474af3e1641c2c20856ea005f45b8cb6abc754cb26 in / 
# Tue, 29 Mar 2022 00:24:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:27:26 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:836a00544655c89c89efabf058adfe305cc708f5259ae1a48e4f895cb836a2b2`  
		Last Modified: Tue, 29 Mar 2022 00:37:55 GMT  
		Size: 60.2 MB (60217263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135952d05ab8fce78c42c34b40a55fd5cb25572c58ef3c4c5bd84a060d9ec25`  
		Last Modified: Tue, 29 Mar 2022 00:41:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:58f0ab0654059d92993cbb7d48f309941d00bc661cabcad318204d91c859fe6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54056676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f810bfa8f6ac4e0d3cf63705077fd64f5f3ef948665c84c87c8ee337d8574a2a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:53:06 GMT
ADD file:5143c5815a4282433726df7dd89926b3676994be1b8575d259b8fb48d6a6a4de in / 
# Tue, 29 Mar 2022 00:53:09 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:54:51 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c86b61bc0bc235576e3d7696ce7a1c21762146f539dc6eda8173ad30b9a4ad20`  
		Last Modified: Tue, 29 Mar 2022 01:16:39 GMT  
		Size: 54.1 MB (54056452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9df048f60ab1b9c1a3c05648e74da20cafa20ddeb40719aae6967c38d65ce7`  
		Last Modified: Tue, 29 Mar 2022 01:32:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
