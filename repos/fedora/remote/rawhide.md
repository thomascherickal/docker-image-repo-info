## `fedora:rawhide`

```console
$ docker pull fedora@sha256:32849b7713f463432b7ddffef285f3464c5df386e1f686f1f974ff4ee940760d
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
$ docker pull fedora@sha256:d9118d70df6443c07f616b82e210567f4c16c5a806e43d2bddf2a1338115ba91
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.0 MB (57968283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7b3bee862521dae2253de5e8ef46df10a3370dffa895a8305681fbbfe1a73c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 01 Apr 2021 18:00:32 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Fri, 01 Oct 2021 23:02:57 GMT
ADD file:66e7def7f748f55d28240be7c22b6a5091881f220bac3f3fa6fb4150b72a21b3 in / 
# Fri, 01 Oct 2021 23:02:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:97458595fadc70d8375d262570f72aa345abb37d2ad63b5afb3119e6bfc44a31`  
		Last Modified: Fri, 01 Oct 2021 23:04:14 GMT  
		Size: 58.0 MB (57968283 bytes)  
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
$ docker pull fedora@sha256:6cef51bfef42d0d93eba46ac18865127688b1e7305f0f681647312a3cfe11e4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55416957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba85dcf68634f46e2252d619cf06c8f6147a05adbe65ca4ffb686f8edb497f88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 01 Oct 2021 22:42:38 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Fri, 01 Oct 2021 22:42:42 GMT
ADD file:2ad915790ee07c5526c02c099a4e87c5b3e8a1cd9d18417cd6beb0cc92772bcc in / 
# Fri, 01 Oct 2021 22:42:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5b4411df31ea2b2120251020a572a65926d8941708d23204447c5a33c028d996`  
		Last Modified: Fri, 01 Oct 2021 22:43:52 GMT  
		Size: 55.4 MB (55416957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
