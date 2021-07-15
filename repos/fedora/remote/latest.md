## `fedora:latest`

```console
$ docker pull fedora@sha256:f534c437436eb44b7ac73646e642732fc055a75d84f900f07c3bbaa392007810
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
$ docker pull fedora@sha256:6c8b3dea130cfa28babcb4d73450ed64f962e5464ab191bc0539487daf25d533
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64929312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055b2e5ebc940affa3a6e0372b8e7f3c33a5db860173c3328ae36a10cfbe30f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 01 Apr 2021 18:00:19 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Fri, 14 May 2021 17:20:54 GMT
ADD file:f8b822814d179a7672f993703092ce712247a57be0e2bb31dfbec263041983ff in / 
# Fri, 14 May 2021 17:20:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1495d80d5267d492823f0904735a9bfabb31db73622e0feca7eb53b566acfd1`  
		Last Modified: Fri, 14 May 2021 17:21:53 GMT  
		Size: 64.9 MB (64929312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm variant v7

```console
$ docker pull fedora@sha256:b521cf9c8233fdc78120a56de0ca1d6d46c16b1e172b8fa54446da52d6b33379
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61226800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a6ba5f947147fc420a0c9897d66c6eec915dadab99561d6e0705f800b804854`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 09 Oct 2020 21:02:51 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 01 Apr 2021 18:03:11 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Fri, 14 May 2021 18:07:17 GMT
ADD file:6bef60588e9fb1a6f4cfb76300ca8924b980d25a8c308245ae9d078590a2fc37 in / 
# Fri, 14 May 2021 18:07:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a367c2737400d51ba4fabcd91f609374934667165f4676c4845f3be7a49c3e57`  
		Last Modified: Fri, 14 May 2021 18:09:32 GMT  
		Size: 61.2 MB (61226800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:43cad8a861e8674e767bc963bf6c71e6399041af3534317d4ae182e53798fd24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64584400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b037572569bf273ac4efbed7196d31f3a98bf0b52c435b48fae2f954ab9b3d9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 18 Feb 2021 22:52:42 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Fri, 14 May 2021 17:57:34 GMT
ADD file:fd15fefa8d187914ed47482f6cbe6fd2d5ca90252aa3f1eb15ea4efcf86490d9 in / 
# Fri, 14 May 2021 17:57:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e834a7f2e69aabed75cd7bf39513aa72060cb1746fe916609dc80983aa143cce`  
		Last Modified: Fri, 14 May 2021 17:59:09 GMT  
		Size: 64.6 MB (64584400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; ppc64le

```console
$ docker pull fedora@sha256:f9accb359b1cbb461b908c66b63e9f86d622b17759d4f4b733b3e0c1f24b6460
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70685915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd3b2004b4b49af07096ea30129744f1c887a1db9e7901f2c39a9629855b8303`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 23:19:06 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 01 Apr 2021 18:18:48 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Fri, 14 May 2021 17:38:59 GMT
ADD file:80539c5ef570057462dec224a4770a5414b47c917aa2508f90384789b443e9da in / 
# Fri, 14 May 2021 17:39:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1e4253e57b8478d2f7787e62a0807b5b04c748fba64de84d75812fddda71b5b6`  
		Last Modified: Fri, 14 May 2021 17:40:45 GMT  
		Size: 70.7 MB (70685915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; s390x

```console
$ docker pull fedora@sha256:c2410e0b4afba1cecf0db2366b03f206de2b14083fc7cda539bcd1a7616f8d6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62446089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfe45c024aa09ed769a77e4382b1c7d11ef7f5757a20060afe7d6875c435131`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jan 2019 12:43:09 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 01 Apr 2021 17:59:16 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Fri, 14 May 2021 17:42:29 GMT
ADD file:63c51fcda8ffe0ed1b267e968f30990c1d8477e72bce5ef29b1b1757d419b2a9 in / 
# Fri, 14 May 2021 17:42:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a81753b6480e1babf723a16a4ef72d16ccfcee3ba45994050177113bd02bf246`  
		Last Modified: Fri, 14 May 2021 17:43:08 GMT  
		Size: 62.4 MB (62446089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
