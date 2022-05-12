## `fedora:rawhide`

```console
$ docker pull fedora@sha256:4d0f1dd7fd1cd2f889824f7d6bc7addc8e24fdf65f6ad209f420ded311505f20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:8424686c5327e302f17f336af82da620eee70b5718a1dd3a44c1e502cc7a59da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59409374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbcdba45a3e72c8a34c1f722f7c2ea2aea4e07ed22d334b84d9ad9b6b095cd56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:14 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Thu, 12 May 2022 18:23:07 GMT
ADD file:29ed98fcf2a35ae3f972a5a6b57dcd9ff6a4499139213bfc0ce0b8c2de02a3ec in / 
# Thu, 12 May 2022 18:23:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:faa6135057fd7d4495c4bbeedd1e53d256c6d3046551a85826db41f787322fb7`  
		Last Modified: Thu, 12 May 2022 18:23:49 GMT  
		Size: 59.4 MB (59409374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:7e33ed23e889cc12d7d7fe9371b87cbce38edc2dc2066c23ae8d4b706e07c587
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57543771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176f23e0e23ecda680c879cb6fff3b6b32f5b797c77c092a4908064101d52e4b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Nov 2021 21:12:33 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 19:19:54 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Thu, 12 May 2022 18:43:11 GMT
ADD file:3b01ffec97301acb3e56352a5592e4f902d6595e013f48728c9fa2e67f53e965 in / 
# Thu, 12 May 2022 18:43:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1c920871d1aa8a278153c3e7d9e80e1939bef56385c6efb8a90fbbf991c4289`  
		Last Modified: Thu, 12 May 2022 18:44:02 GMT  
		Size: 57.5 MB (57543771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; ppc64le

```console
$ docker pull fedora@sha256:f396a8b214bcab8702405906e248ce309c7bc35c9501a0bea358f8f1aad4da6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64802535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7190720ce9ae16d5674b7334201bb55884459b1cb4d8ee87289f9c277943166`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 23:32:50 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 04:53:18 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Sun, 20 Mar 2022 04:53:26 GMT
ADD file:d67c1cc8c3ae4d10c61bb05df49aa2bc24fc0c12fd28c701e0f414d72eae76be in / 
# Sun, 20 Mar 2022 04:53:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:67f00d7364ab8ac6421ca2d6c6e01d4a6ddaebd166a823a60025e118a5b3d7cd`  
		Last Modified: Sun, 20 Mar 2022 04:55:29 GMT  
		Size: 64.8 MB (64802535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; s390x

```console
$ docker pull fedora@sha256:8a746cdc3af9334bcbf48be4bebfc6d6428af817e6e886b26f495b718c666911
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56500892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69f754d5d0de1955e685cf252d714b6acc593b9ced3f6a106958ca68c64d50e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 04:31:50 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Thu, 12 May 2022 18:43:48 GMT
ADD file:3f10131e3bc0caa9a0206a822c9896790eac5b35bf4ac1accb5652f1cef842ee in / 
# Thu, 12 May 2022 18:43:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1163606821de65d610cb57b7fd309908cb7b5d049fa1c4fda6773be2e54e5628`  
		Last Modified: Thu, 12 May 2022 18:44:39 GMT  
		Size: 56.5 MB (56500892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
