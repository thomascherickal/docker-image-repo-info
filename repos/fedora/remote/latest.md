## `fedora:latest`

```console
$ docker pull fedora@sha256:f1e3a29da8990568c1da6a460cf9658ee7e9b409aa39c2aded67f7ac1dfe7e8a
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
$ docker pull fedora@sha256:36af84ba69e21c9ef86a0424a090674c433b2b80c2462e57503886f1d823abe8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54630347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97d90f26110930f4ea32c16be938ecac6f85b5b917edf1390e0dcf8f467bd33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 01 Oct 2021 23:02:34 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Sun, 20 Mar 2022 10:45:51 GMT
ADD file:8f4c7115559a78277879657b79ebcd463a96e7ef86e1d80f6fa3a6ece3a8fec4 in / 
# Sun, 20 Mar 2022 10:45:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:054e3e802ba7bde57dcc19df7b12ac4fecb92bc0c3e7b591210bcea96f993b5d`  
		Last Modified: Sun, 20 Mar 2022 10:46:58 GMT  
		Size: 54.6 MB (54630347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm variant v7

```console
$ docker pull fedora@sha256:e576ebd3ec779d2bfae418ed723be9ba7dfb9cdafc1a03dea6f9d511371ddab0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51355675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a474422f8a81a8da2dcef2ddeacf2d66b20ed6e66a2dcb76dd168e0ec4a198c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 19:03:21 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 02 Oct 2021 18:49:21 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Sun, 20 Mar 2022 09:15:03 GMT
ADD file:126156355713512eb4dcf8a5c74f98cfee582ab1009b6a2ebb7f80df18c1cf04 in / 
# Sun, 20 Mar 2022 09:15:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a15b8bae470bd37a7407e54b1c65921b9bac5bd4e7f29c6b2bf43c3102058a78`  
		Last Modified: Sun, 20 Mar 2022 09:17:37 GMT  
		Size: 51.4 MB (51355675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:acf39c9fb7cd0fa51ee423f9536667007a1b52e98c6030c823007cf5686c7765
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53608583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775b4cdd6b58e0dd0077142af08f123c9ed90ac24c4004f161afd01f86c3c95b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Nov 2021 21:12:33 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 02 Nov 2021 21:12:58 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Sat, 19 Mar 2022 19:19:32 GMT
ADD file:a7d0a8d9a9133b3614c6961097e462a1e98ed32bd2a7d73f21552362e625edb0 in / 
# Sat, 19 Mar 2022 19:19:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:623fc6c8f399e6dde93fc82beed08af10e667fa3896b48d4d41b3f93d652dd0c`  
		Last Modified: Sat, 19 Mar 2022 19:20:45 GMT  
		Size: 53.6 MB (53608583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; ppc64le

```console
$ docker pull fedora@sha256:661ef6f75b0f86e80fed7f9be624ff9468b757aa6e27104560f93d32ae9c49cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59506548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8293b5f08e53e3b9adc782fa0ab04bade6234b5537605c4fab412b93df38779c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 23:32:50 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 04 Oct 2021 19:40:14 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Sun, 20 Mar 2022 04:52:29 GMT
ADD file:25605fa3c15c4b8ebc4503ffcae3426a01883ee0f165066f43c3142a89a3d687 in / 
# Sun, 20 Mar 2022 04:52:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9a673a4aa047e8607810cc1bbd52772ae4fd70ec5b6e3031bfce17b2a04b7589`  
		Last Modified: Sun, 20 Mar 2022 04:54:40 GMT  
		Size: 59.5 MB (59506548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; s390x

```console
$ docker pull fedora@sha256:3d63aa1da663b274bf158281d07e77db1e7b199116aac54f1bc7175c856a937b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52571418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b6c80727783f4c6c0668e3c208f9f77a15c86986799066ce6c1139f5587ac6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 01 Oct 2021 22:42:23 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Sat, 19 Mar 2022 04:31:18 GMT
ADD file:e08d7b2813b14e6ceb9044105795f7f567a3346596ba733cd7e50607d0b21f99 in / 
# Sat, 19 Mar 2022 04:31:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:068a470be0289c24db02bcbfc57bd4bc7fce673b9b1f6da92a0807e164713882`  
		Last Modified: Sat, 19 Mar 2022 04:32:42 GMT  
		Size: 52.6 MB (52571418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
