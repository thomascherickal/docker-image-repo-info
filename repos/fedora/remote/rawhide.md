## `fedora:rawhide`

```console
$ docker pull fedora@sha256:f7e88b3a542eca2fe0c7b700931aa09645cb7c953838bf6db4fd2893c4c88e6c
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
$ docker pull fedora@sha256:872ce99cbe662261de3b107a001c4b41e2253f06faa0efe81c4fdc4fa73f8fc5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61643977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:500fd4b5ebe9d930fc28da7ad9a7d3ed87ef1bace5db00767b9e205bdebb2882`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 25 Aug 2020 17:46:51 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Tue, 25 Aug 2020 17:46:59 GMT
ADD file:2ffb6c7f0afd8a3d319d4faeadd37716d649b9aace3b69ef28f27a8fcdd84b6b in / 
# Tue, 25 Aug 2020 17:47:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:567c5e83e195d401a1a58236e1788fa5a68f7144da38b0ac8af41b7b7d881cfc`  
		Last Modified: Tue, 25 Aug 2020 17:48:02 GMT  
		Size: 61.6 MB (61643977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
