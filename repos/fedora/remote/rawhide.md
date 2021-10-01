## `fedora:rawhide`

```console
$ docker pull fedora@sha256:5dbb515fe91d38d54e42fbecabd99606bad97293b4ccb81e3a63ba132a5d136e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:6382c102ebbdfcb137f6048c3e5aa964db0c4882b8b9eb8ebdaf52620935b7ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65548170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2f5884f8581640b952e750e6673c8ea71a97e709c567a8aaed6648753e1c111`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 01 Apr 2021 18:00:32 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Fri, 23 Jul 2021 11:16:18 GMT
ADD file:3af0cad5aa27df35a951f0781998a97aff5e28443f7c9eecb6d7c74fd84e921d in / 
# Fri, 23 Jul 2021 11:16:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fc972fbab1a5944103b867e535959227bbc28e43e19827d51668d3169547a4ba`  
		Last Modified: Fri, 23 Jul 2021 11:17:19 GMT  
		Size: 65.5 MB (65548170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm variant v7

```console
$ docker pull fedora@sha256:507370aea886052d775472239c94ec5ec94edfd6f45ffed03f04c02bf024f289
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62181496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9da0b58d5a841d2c661d8e8775c710177bda9751f9ba917d82882b1ba2c0754`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 19:03:21 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 23 Jul 2021 19:05:03 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Fri, 23 Jul 2021 19:05:20 GMT
ADD file:03c922c247e780c5ec7b8ad76ae85101f73d53fc5962c213016ea1b346e08943 in / 
# Fri, 23 Jul 2021 19:05:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0cc98a41e61789633667eb6a62db9a061f0bad483f6c74b66ce31e0f5b5137e7`  
		Last Modified: Fri, 23 Jul 2021 19:09:08 GMT  
		Size: 62.2 MB (62181496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:8ff38f5db341b4322e14ca9ea7a5e78f62b42188926688f54b0501456c8a4d32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65473773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1373194a928125016b1e0e08872b974c608e16a7070113669bf6524beeb7228`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 01:32:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 23 Jul 2021 01:33:02 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Fri, 23 Jul 2021 01:33:07 GMT
ADD file:f73b3b52739eaeba7350f82df39731405eaad0d4e68d68dbe22f4b9f94703bf4 in / 
# Fri, 23 Jul 2021 01:33:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5cc6411571192f63b9ac80c6771226bdd30fbaec9f49f93ba8b75f958bf7f1a8`  
		Last Modified: Fri, 23 Jul 2021 01:34:40 GMT  
		Size: 65.5 MB (65473773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; ppc64le

```console
$ docker pull fedora@sha256:8e1c7a34e4a3e1f606e3e0ee3794ff4a8f2a53d549a9a5ca049ddc4e0f9a06de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72575604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f84dac3f1b550a0a569a59ba9c13dc9c3cb3e41eceecfc71c25381ba748d92f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 23:19:06 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 27 Apr 2021 21:28:25 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Tue, 27 Apr 2021 21:28:36 GMT
ADD file:23d27bab5e0d22617d315811ee0be53762a59c8ae15b69dd5d6d60ff465aa036 in / 
# Tue, 27 Apr 2021 21:28:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:aa0cf73e1f99c7d46f73e0fd5ca1f45a3a8aaf7b828f46de9976703dcd9b34c9`  
		Last Modified: Tue, 27 Apr 2021 21:30:16 GMT  
		Size: 72.6 MB (72575604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; s390x

```console
$ docker pull fedora@sha256:0d8cfed5f02e5b9e1be8d8722cd522f1c1174c1bbd9fa111fe18ef20c6ae073c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64366662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd9d2a110ebfeb85ac147d2df689b6e0fb209fe5c12a48a368914e164778a4b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jan 2019 12:43:09 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 27 Apr 2021 21:43:47 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Tue, 27 Apr 2021 21:44:03 GMT
ADD file:8c9f726d30bb653a7e5069a19435706f92292779021cee57c31a7fbd62f9bd4c in / 
# Tue, 27 Apr 2021 21:44:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:efbdded58a6ec9d58cded5105a8a1b8379fe84baee38bb42cf6452cca0936684`  
		Last Modified: Tue, 27 Apr 2021 21:45:28 GMT  
		Size: 64.4 MB (64366662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
