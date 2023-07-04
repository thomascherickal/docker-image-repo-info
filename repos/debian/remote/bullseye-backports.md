## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:acf4f59e1d72ffd8dad79ba88aa2c6c99f99d16cd2fc11bc8129c49351518d38
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:f5ec299e3f1fc6ba27a2d066becacbbb061cead756898b1a2a6d900542351524
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55055525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39783992e08db2f199d8f2830b05bca644456b69c1930771bb97449a246abdbc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:20:14 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa19a1e07459e404e7712c9a2f50e0a015759f9ad59341c5884c6284707b1acb`  
		Last Modified: Tue, 04 Jul 2023 01:25:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:44fbc710ea5fc0538cacc1ca4d5d192f664aee11815d58f159bd50b136a02004
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52557003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9281d9310ac3c181ee076f1b68a43c994205fb260ef016599e4831f2e15595d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:48:42 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a170a2cf9bb1b9df44ef8581288cd8db7c03094b0c792d6b5ebcd6beb1866`  
		Last Modified: Tue, 04 Jul 2023 00:52:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:5767bcea30c0706e7083ef279d998f5ce0a11251a1735e9e7efe53b4dd5e3c42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50218471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be6b17bb9d70c83abff33da7de1d326f8e26c7538f7ac14565670579c969de9e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:58:10 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c11575019926ec464a3c162c92a4efa5ff0ac05a431f177207d025823bf40d`  
		Last Modified: Tue, 04 Jul 2023 01:03:24 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:dc13e89735df155c95ffb9c2e115c6803783604370fab26a8ed450bedea9e7f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53704363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9577c0c740ff9200ec1d0d063161763abf8636ef230b2190d978a418645a8c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:40:26 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13335849095b09b95196e329330613112fc0c8e6f93eaa1c1623c2bae2ecff4`  
		Last Modified: Mon, 12 Jun 2023 23:44:37 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:c5e4f5e031f5c36e5ce62fba93999c16010ed25cb2e8b328fce5d30238c9e46e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56040888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3c7107d65d03d0f5a4ef8852a25ead5f744ef9768e4841c2f88268129f9858a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:39:44 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8578475b3f3c61a99ae8bc61e58c89b331148c52e806854a5d93af64499731`  
		Last Modified: Mon, 12 Jun 2023 23:46:55 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:2753db08a096867fc24aca53dafacbaafc1dae6c974f4d2af5847e3a8fcf8a3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53270697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7505d71f35126ee712f62b7d1caccf4bc39787f8d0b4fdd599aa665604b1efdb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:02 GMT
ADD file:f7ddd7406e3aa24165fc80933583fc2298f9792865511fe65def2f571fed2207 in / 
# Tue, 04 Jul 2023 01:10:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:10:21 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:af98e96208d7ce4cff5417a3e8a38f98d2ed3abbca318e1e6c323aa8b8c56690`  
		Last Modified: Tue, 04 Jul 2023 01:20:40 GMT  
		Size: 53.3 MB (53270472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f6fb1c2fcb080f03a61eef6b0e20b57f4684e328f00202d760bfbfd0a8f043`  
		Last Modified: Tue, 04 Jul 2023 01:20:55 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:daa80aed4b5deaf2c5ba864a01b6eca4d3f9c7858df86e0ffd4d4b455e37293b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58927973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd7e8da683dd895282628eb901a0dbf95d47f5744255afe4f39869ff4f77e382`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:11 GMT
ADD file:ff86c25854c28609c2852c1615270f0acd4c4efaa38ff8ed9c23afe5132f2135 in / 
# Tue, 04 Jul 2023 01:18:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:18:20 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a792749f62225048efdf85841bea6f3999f586371852f3dbce13a6c3d89b1fa7`  
		Last Modified: Tue, 04 Jul 2023 01:25:06 GMT  
		Size: 58.9 MB (58927745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c434ee1d4ac272227206ff97f81558cb557407d9ae335b6c4cc1ffa260adfd5`  
		Last Modified: Tue, 04 Jul 2023 01:25:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:40e24833703a4cb2ca57ac72544e4811ea8a531c35db7937268e9b09ce3c5215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53288266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be0643f3f5944dbfb232af639c32bf1e5940e44e72703a0daa1a5daef948967`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:54 GMT
ADD file:fa60f19da2df43542549a5dd89b364d30fff981d1655f9cce8900778a7b841b9 in / 
# Tue, 13 Jun 2023 04:29:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:30:03 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2bef9d7959742dda03e39c77232808f6559cd696f21fab76fc714bdd24cae18d`  
		Last Modified: Tue, 13 Jun 2023 04:34:33 GMT  
		Size: 53.3 MB (53288042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356b63e648326d46d6e78bc360e8f26ece851b3451f4cbda4836a2d6f1890b11`  
		Last Modified: Tue, 13 Jun 2023 04:34:41 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
