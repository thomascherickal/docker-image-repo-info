<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20220918.0.86346`](#archlinuxbase-20220918086346)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20220918.0.86346`](#archlinuxbase-devel-20220918086346)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:48806dfa92c35733e3d60435448fc8aa3fedf0cba96fcbad7afc47b2b1fc20e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:2cc0c392d7d9df6a437b3e43f2588ee3692dc73b001d2c552b8e47c74c0d93ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138556957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f1632cc0df0f34b2c43f46c8798bc99be0651b1e783a7c7b9f1fb3fd28193d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 19 Sep 2022 17:42:30 GMT
COPY dir:05a4953f90b0a55224fcfdf93d3ce965c2fac9bc38dd813d3eb3086b3ea9a5b6 in / 
# Mon, 19 Sep 2022 17:42:32 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 19 Sep 2022 17:42:32 GMT
ENV LANG=C.UTF-8
# Mon, 19 Sep 2022 17:42:32 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:c3298b3c36558f264f05f3c3b6308bcd7c89967eba2693dcaa52604b182f6db7`  
		Last Modified: Mon, 19 Sep 2022 17:44:15 GMT  
		Size: 138.5 MB (138548856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8518d59169bdd707ed1114bf9c4e7a0ff58862d147068bacd203d80588bb7bd1`  
		Last Modified: Mon, 19 Sep 2022 17:43:54 GMT  
		Size: 8.1 KB (8101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20220918.0.86346`

```console
$ docker pull archlinux@sha256:48806dfa92c35733e3d60435448fc8aa3fedf0cba96fcbad7afc47b2b1fc20e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20220918.0.86346` - linux; amd64

```console
$ docker pull archlinux@sha256:2cc0c392d7d9df6a437b3e43f2588ee3692dc73b001d2c552b8e47c74c0d93ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138556957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f1632cc0df0f34b2c43f46c8798bc99be0651b1e783a7c7b9f1fb3fd28193d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 19 Sep 2022 17:42:30 GMT
COPY dir:05a4953f90b0a55224fcfdf93d3ce965c2fac9bc38dd813d3eb3086b3ea9a5b6 in / 
# Mon, 19 Sep 2022 17:42:32 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 19 Sep 2022 17:42:32 GMT
ENV LANG=C.UTF-8
# Mon, 19 Sep 2022 17:42:32 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:c3298b3c36558f264f05f3c3b6308bcd7c89967eba2693dcaa52604b182f6db7`  
		Last Modified: Mon, 19 Sep 2022 17:44:15 GMT  
		Size: 138.5 MB (138548856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8518d59169bdd707ed1114bf9c4e7a0ff58862d147068bacd203d80588bb7bd1`  
		Last Modified: Mon, 19 Sep 2022 17:43:54 GMT  
		Size: 8.1 KB (8101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:61d07c024369c0d66ad1fdb1a72849f401cc1d06e997800b50a84d9998ee517a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:c94a2633b402d2cf07343564a44b852b7ef1758af70d53edd13b697bac022a05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236824083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edad53189e9ee56eb28443e3c7fe9b7d7e68cf423a3af5ec58a66f70bd688f85`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 19 Sep 2022 17:43:31 GMT
COPY dir:7a9f55aa3b47cf7267a8485c8101c9aa85637105151f39346dcfe8a465dd9744 in / 
# Mon, 19 Sep 2022 17:43:34 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 19 Sep 2022 17:43:34 GMT
ENV LANG=C.UTF-8
# Mon, 19 Sep 2022 17:43:34 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:16a106e71ce5d7f920ae07e9d1d92e3b2da4ce2eada6f9df3f8839c1e3ca7679`  
		Last Modified: Mon, 19 Sep 2022 17:45:02 GMT  
		Size: 236.8 MB (236815311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e970fddd4fb5debb710a45d3dc67b8b425b7deb760c33292817d6f6e2c0140c8`  
		Last Modified: Mon, 19 Sep 2022 17:44:26 GMT  
		Size: 8.8 KB (8772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20220918.0.86346`

```console
$ docker pull archlinux@sha256:61d07c024369c0d66ad1fdb1a72849f401cc1d06e997800b50a84d9998ee517a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220918.0.86346` - linux; amd64

```console
$ docker pull archlinux@sha256:c94a2633b402d2cf07343564a44b852b7ef1758af70d53edd13b697bac022a05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236824083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edad53189e9ee56eb28443e3c7fe9b7d7e68cf423a3af5ec58a66f70bd688f85`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 19 Sep 2022 17:43:31 GMT
COPY dir:7a9f55aa3b47cf7267a8485c8101c9aa85637105151f39346dcfe8a465dd9744 in / 
# Mon, 19 Sep 2022 17:43:34 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 19 Sep 2022 17:43:34 GMT
ENV LANG=C.UTF-8
# Mon, 19 Sep 2022 17:43:34 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:16a106e71ce5d7f920ae07e9d1d92e3b2da4ce2eada6f9df3f8839c1e3ca7679`  
		Last Modified: Mon, 19 Sep 2022 17:45:02 GMT  
		Size: 236.8 MB (236815311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e970fddd4fb5debb710a45d3dc67b8b425b7deb760c33292817d6f6e2c0140c8`  
		Last Modified: Mon, 19 Sep 2022 17:44:26 GMT  
		Size: 8.8 KB (8772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:48806dfa92c35733e3d60435448fc8aa3fedf0cba96fcbad7afc47b2b1fc20e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:2cc0c392d7d9df6a437b3e43f2588ee3692dc73b001d2c552b8e47c74c0d93ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138556957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f1632cc0df0f34b2c43f46c8798bc99be0651b1e783a7c7b9f1fb3fd28193d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 19 Sep 2022 17:42:30 GMT
COPY dir:05a4953f90b0a55224fcfdf93d3ce965c2fac9bc38dd813d3eb3086b3ea9a5b6 in / 
# Mon, 19 Sep 2022 17:42:32 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 19 Sep 2022 17:42:32 GMT
ENV LANG=C.UTF-8
# Mon, 19 Sep 2022 17:42:32 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:c3298b3c36558f264f05f3c3b6308bcd7c89967eba2693dcaa52604b182f6db7`  
		Last Modified: Mon, 19 Sep 2022 17:44:15 GMT  
		Size: 138.5 MB (138548856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8518d59169bdd707ed1114bf9c4e7a0ff58862d147068bacd203d80588bb7bd1`  
		Last Modified: Mon, 19 Sep 2022 17:43:54 GMT  
		Size: 8.1 KB (8101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
