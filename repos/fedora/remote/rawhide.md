## `fedora:rawhide`

```console
$ docker pull fedora@sha256:10de9fde508b71568da7d3d05edde5780de40851ff3f03b7697e5d240e3d609d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:3f94fa91a3dbe38e4425f01d4575bd9b448aa87de00a4f854459dd056c32925b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69513650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9288358f6f5b55bdde4f4090611d2b8e1403845226a0fa321a1475d3b234dd6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 13 Mar 2023 21:20:05 GMT
ENV DISTTAG=f39container FGC=f39 FBR=f39
# Wed, 31 May 2023 17:23:59 GMT
ADD file:f6004eb95608d199e649218d5e6560d2355d65bb5da4dd027506f60c16d90d29 in / 
# Wed, 31 May 2023 17:23:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:adc0d05c6919dd118e9f4e41b239c6ac6c1f5fc42ce88941452f84c1cdc94287`  
		Last Modified: Wed, 31 May 2023 17:24:52 GMT  
		Size: 69.5 MB (69513650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:9e726e3052bdb633096b4d84f9d29082aac3def4f630c5ce6226b166c226f144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67205357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d46dac57db33f4823ff624d7187f37a3d7e0a619a03a5e693696b1b0fffd524`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 13 Mar 2023 20:39:50 GMT
ENV DISTTAG=f39container FGC=f39 FBR=f39
# Tue, 06 Jun 2023 19:40:14 GMT
ADD file:3e6cf1e39ef84e98a1b3dfd08275fc07a29f0d898d30849b178d0c04bfad21fd in / 
# Tue, 06 Jun 2023 19:40:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:91dc871cee77c64af13bb6bc2db01ef886031f113319c4c7393546f649f420d7`  
		Last Modified: Tue, 06 Jun 2023 19:41:00 GMT  
		Size: 67.2 MB (67205357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; ppc64le

```console
$ docker pull fedora@sha256:d62c889e11d0ba1dd5300800e4be6d095bbeca929e94b74accfa1268230a44e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76258495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9814fafc47c5fdae70b42febd33a54c62f689356d7f03894072f9a50cb90d990`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 13 Mar 2023 21:18:04 GMT
ENV DISTTAG=f39container FGC=f39 FBR=f39
# Wed, 31 May 2023 17:17:49 GMT
ADD file:8a981bddf8e6cfa5f4563f841b8ac9be6d35bb6591df6640bd0ce118daa7bfe5 in / 
# Wed, 31 May 2023 17:17:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1f9b0c4ce288662f3b408f34a7f0df6ff46f00e19015f3b79ba5627aaa3ce220`  
		Last Modified: Wed, 31 May 2023 17:19:16 GMT  
		Size: 76.3 MB (76258495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; s390x

```console
$ docker pull fedora@sha256:becd91c0914bfb8471905050c87570405a2c6d7eb146fa2f89058e7cf3a959d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69163305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3e509c578d23da614b51f89b21654af9274e10174f6c492b02a3917587a342`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 13 Mar 2023 20:43:12 GMT
ENV DISTTAG=f39container FGC=f39 FBR=f39
# Tue, 06 Jun 2023 19:43:17 GMT
ADD file:9450db2cf55b9a98d578379905b5de508c7dff0d20b834c46ea97a5420228a09 in / 
# Tue, 06 Jun 2023 19:43:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:27c1534f45586ad09aba8c625a388bb389e5d9fa9e861a96d8e4a29cd94a612d`  
		Last Modified: Tue, 06 Jun 2023 19:44:06 GMT  
		Size: 69.2 MB (69163305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
