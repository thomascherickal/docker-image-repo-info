## `fedora:latest`

```console
$ docker pull fedora@sha256:a1a130195520b4a145c6bef0f247024f76bee573e48af130e5e1296ca769cfdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:latest` - linux; amd64

```console
$ docker pull fedora@sha256:1bb4d23fb3b90037d55e74498a77da2c3e6b37f879db3ce14eb1e7c9a3adaf4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64825663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81c8ae4dda7dedc0711daefe4076d33a88a69a28c398688090c1141eff17e50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 13 Mar 2023 21:20:05 GMT
ENV DISTTAG=f39container FGC=f39 FBR=f39
# Mon, 06 Nov 2023 23:27:35 GMT
ADD file:1b2b17e6070e418b4005c37e01b3b1b54144df4a2844e1119c63cdfda27c3d6b in / 
# Mon, 06 Nov 2023 23:27:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fdb62196b28f3c7729a582231858ddd134233b54e24e208e16232585db6af13d`  
		Last Modified: Mon, 06 Nov 2023 23:28:39 GMT  
		Size: 64.8 MB (64825663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:780bd12b0538bcffeed648f4f33997323f7141b1f401aaef0881f46177cc003d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63463925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b48f9d1afbb17f091109a9a183730432d8ed44d2768f7f461b7a7c662bb986e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 13 Mar 2023 20:39:50 GMT
ENV DISTTAG=f39container FGC=f39 FBR=f39
# Mon, 06 Nov 2023 23:42:24 GMT
ADD file:cc268a6ca834a14a18c515d6c717ac28a46fdb1e6cb2a2813c9622b52e5d375e in / 
# Mon, 06 Nov 2023 23:42:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:032b04d14cd737ae07fb9283264a6c7a5551be832b5b1210e7a3ce5964eea869`  
		Last Modified: Mon, 06 Nov 2023 23:43:19 GMT  
		Size: 63.5 MB (63463925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; ppc64le

```console
$ docker pull fedora@sha256:1e6d8d678e832d9b14fc5f4f013781ac7e8c5cccdb2d5ed8efa852ca90ac1fc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75665507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664d91615f3cb656f62a2c648ca5f9b275e5e125f03db217ce23e979fbc55493`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:19:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Fri, 06 Oct 2023 18:19:54 GMT
ADD file:1819574642d8ac7663def1ece7a7276d16b5d98260dffc58a3ddf27bf4b93e8a in / 
# Fri, 06 Oct 2023 18:20:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0354f7434cd95c31bcb66d02a186d70ffb7de5c65c00e52ec68c0a3dfef73cf9`  
		Last Modified: Fri, 06 Oct 2023 18:21:46 GMT  
		Size: 75.7 MB (75665507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; s390x

```console
$ docker pull fedora@sha256:53893c9113948b87c0da7fef43c3cde3919cf4bae890203056bf4cb64eab10ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65358613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:081f9c817e2553a2bf1e3cdbbb0d08e0e41cedc023a189401896784e370c8ce5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 13 Mar 2023 20:43:12 GMT
ENV DISTTAG=f39container FGC=f39 FBR=f39
# Mon, 06 Nov 2023 23:44:42 GMT
ADD file:5c1fb01e7997c8bc5043a7e671a4f34a7faea6f120ae2224a9a8b4c7217f0cd9 in / 
# Mon, 06 Nov 2023 23:44:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2519a55acdc41056e791d9604f41fc86557f884eb5939a1ccad5cf0961d61ca3`  
		Last Modified: Mon, 06 Nov 2023 23:45:54 GMT  
		Size: 65.4 MB (65358613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
