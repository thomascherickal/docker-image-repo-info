## `fedora:latest`

```console
$ docker pull fedora@sha256:72c6c48a902baff1ab9948558556ef59e3429c65697287791be3c709738955b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:latest` - linux; amd64

```console
$ docker pull fedora@sha256:db8380e69336e37a94bacad856abfde03cd7060f53530be1c7de32526b00dfd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54779887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b080de8a4da3da9ec2fdbeeb6d70d94079b27df87483039fc45abd2152109c43`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 01 Oct 2021 23:02:34 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Tue, 02 Nov 2021 21:29:21 GMT
ADD file:be45b9d0e66aaff43304ea2300127b0027e748b263fa26d203cd7012eddf7d19 in / 
# Tue, 02 Nov 2021 21:29:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fc811dadee2400b171b0e1eed1d973c4aa9459c6f81c77ce11c014a6104ae005`  
		Last Modified: Tue, 02 Nov 2021 21:30:16 GMT  
		Size: 54.8 MB (54779887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm variant v7

```console
$ docker pull fedora@sha256:e82204d97e6f84155f20a6644864f2a30a8ac0193d00eb31e5427b1ff11bc043
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51458022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56216e9f4d1dc523252090c1fa10428885af2b1533ad1fb0c008ed42411e6f28`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 19:03:21 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 02 Oct 2021 18:49:21 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Tue, 02 Nov 2021 22:56:07 GMT
ADD file:b6bb687b83a6557c55635cc922854e306b9d106bdf59fe4af2e48e7f085fc7bd in / 
# Tue, 02 Nov 2021 22:56:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c4392c845f7cef31de93d83b4b2d94d7a31e4a65d445f2b2b1c18a44022aa194`  
		Last Modified: Tue, 02 Nov 2021 22:58:41 GMT  
		Size: 51.5 MB (51458022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:eb6934c99216962a8860abc8cc38a5dbe26a3a823ca6a646886d02bbb7c90252
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53779450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21f7c65055e723f9afeff807f84236a391f9451c2957bb960e79704fbb70b0e2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Nov 2021 21:12:33 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 02 Nov 2021 21:12:58 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Tue, 02 Nov 2021 21:13:02 GMT
ADD file:f692703c83a7a1b73f3b8481470a706e384ae7e385652a5ffbe604b338f1255a in / 
# Tue, 02 Nov 2021 21:13:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:55bbeef7e282fa3909a3d777b6c2bd2c965627de4d537994838627d5508ea328`  
		Last Modified: Tue, 02 Nov 2021 21:14:16 GMT  
		Size: 53.8 MB (53779450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; ppc64le

```console
$ docker pull fedora@sha256:f8ea92b303c6138d78f9bf54fdf6dd2495b9d0dc4073118a38038522f809cc7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59575956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8a45706d361309316c3078e65e37cab04801078e93a964902635e34be002d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 23:32:50 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 04 Oct 2021 19:40:14 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Tue, 02 Nov 2021 22:46:26 GMT
ADD file:674acdcc535fa5adfec9f763c10e6d300ef041ac207d96ef9da09d1289837415 in / 
# Tue, 02 Nov 2021 22:46:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:aa1933de26af74dd559b4acc8c51450452147d8c8208f0badd081fce540c9332`  
		Last Modified: Tue, 02 Nov 2021 22:47:51 GMT  
		Size: 59.6 MB (59575956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; s390x

```console
$ docker pull fedora@sha256:6d0c2a9d93b142fc01b21e21af644be95b7e6bb5cc0ccbb0382de787e99a26b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52727110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4b4a9b57271af591022ae0dd8f97e3d68a2d61c89f28a5c9a0d9395c3332033`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 01 Oct 2021 22:42:23 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Tue, 02 Nov 2021 21:28:36 GMT
ADD file:21c28fd1d13df6b1e0bb57f883f8351c467ea20e05e8d36d1cc046173040c3ce in / 
# Tue, 02 Nov 2021 21:28:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4ff0313afc065432177e40ce9e640fb0ded68d6be98fdd233a8cec88e2b42b69`  
		Last Modified: Tue, 02 Nov 2021 21:30:06 GMT  
		Size: 52.7 MB (52727110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
