## `fedora:rawhide`

```console
$ docker pull fedora@sha256:4b181cd2a40b557d651a8b8776847517f60ad21e540e81d24a812eeecc32ae6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:8d89b6b3f5d501afd4875a1a250f33e1fddda7b96d5aa5886eeefee8e29612fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65165341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ff04a4b8bd6824e118d512caceffc433bbdd60a02e9f8c1b649968a8fc6f51`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Jan 2019 21:21:55 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:21:44 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Fri, 10 Jul 2020 20:14:07 GMT
ADD file:5465cd6809e79e1be0bbaf7d371fc220edbbd8a46002b6673fba7299ed38ec44 in / 
# Fri, 10 Jul 2020 20:14:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:90cdc03ac7c1ff13eb31ef8b5de9ac2f8c62ad16180a11d2d68cfade36fb7d2d`  
		Last Modified: Fri, 10 Jul 2020 20:15:14 GMT  
		Size: 65.2 MB (65165341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:6b33616281680d5ac0f5a8a4c8cc6bb3f6445d095848506a67a9f2c3ffa94a93
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65384127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deaffc3deae78ff474905e47b189abd81c435268609635749de3bfc727306afd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 30 Apr 2020 23:01:35 GMT
ENV DISTTAG=f33container FGC=f33 FBR=f33
# Fri, 10 Jul 2020 18:52:42 GMT
ADD file:72a91f303cf43e916f97c2f80c34f15940ea7b19ee1067c910e8e6f19297fed0 in / 
# Fri, 10 Jul 2020 18:52:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:525109fb1c3ca2fed333614f70bd8cf97e73503cf4c4eb75f54709dbb41714a0`  
		Last Modified: Fri, 10 Jul 2020 18:54:07 GMT  
		Size: 65.4 MB (65384127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
