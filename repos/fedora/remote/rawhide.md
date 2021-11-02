## `fedora:rawhide`

```console
$ docker pull fedora@sha256:8f826d2b4322fe33d89a49ce21889daf05c5f67e0b0f06c1057d8b021b2021c8
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
$ docker pull fedora@sha256:f7bb300bcb576e73dde5a246d2b19526d43960d1f7eb47c73417a240b7ed35bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57706756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf0d0c364a631bc7dd12c8a1f59d01e4ccca6ffece5bd504e1567d057de92e6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 01 Apr 2021 18:00:32 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Tue, 02 Nov 2021 21:29:33 GMT
ADD file:acf26dfcac681503f9e26a37bb5b068a4759dc0ab17b5f1050593f335314fe36 in / 
# Tue, 02 Nov 2021 21:29:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a029976c022b471b42be8f08d0335b0464dcd02cac8f67209c40ac6e341ab301`  
		Last Modified: Tue, 02 Nov 2021 21:30:34 GMT  
		Size: 57.7 MB (57706756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm variant v7

```console
$ docker pull fedora@sha256:b3fd24fd2c83692d44c3a1875277f975b9dc8e77729129679903fd53d7992e9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53895689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62cded2320283ab500b22a46a9fbb927abcdd4a563b00439f58a515d6453ccd5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 19:03:21 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 23 Jul 2021 19:05:03 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Tue, 02 Nov 2021 22:56:37 GMT
ADD file:f63043a615d0735e7e2c2bb327ee859b139ee786498cf77946621b0d266f224a in / 
# Tue, 02 Nov 2021 22:56:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9f1cd5a19a036e3a24f897dba2456ee68bf2f113bd402d4a32eab45e2583deb9`  
		Last Modified: Tue, 02 Nov 2021 22:59:28 GMT  
		Size: 53.9 MB (53895689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:e68bc50be57ad40bdea883ab3258ef54d31db8f040f566fb94d7c33b2dbbdbee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56500761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f231a68ffe80ee9627d48fd6d094a60ecce03b963e8e8e913b1a8232820a0c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Nov 2021 21:12:33 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 02 Nov 2021 21:13:09 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Tue, 02 Nov 2021 21:13:13 GMT
ADD file:604e2ef3b8dc32d11da1cea3535b660bc595a1edb5f2c1086044bad452f95173 in / 
# Tue, 02 Nov 2021 21:13:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:761f7e0d8b44b3ccf888adc5f0c06915c28cd89cfd49738aa57bd74c6b80fca4`  
		Last Modified: Tue, 02 Nov 2021 21:14:36 GMT  
		Size: 56.5 MB (56500761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; ppc64le

```console
$ docker pull fedora@sha256:c8a8978ab0cd7179f7939b0b90c819c790177d04af9da87c0be8a3f1eb8b6455
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62936147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ad394517791196c73aa8e8409673c0a0edb9fd169c031e46d66832f01fec1b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 23:32:50 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 04 Oct 2021 19:40:57 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Tue, 02 Nov 2021 22:46:52 GMT
ADD file:4588be93eea957e400eab1c1cdc36dc31eb37f882edb87f2c6e83c4fd5025293 in / 
# Tue, 02 Nov 2021 22:46:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:99ad4baf4202d7be14137713425709d4866cb140fb8757e5ba4c49fc1ea36642`  
		Last Modified: Tue, 02 Nov 2021 22:48:15 GMT  
		Size: 62.9 MB (62936147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; s390x

```console
$ docker pull fedora@sha256:afafc77b4632c6750bfffaa099fc8e753b2a38e0496922956e13020cd937203e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55158170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4825a88388dd83c71d7ebe46b8bbcd412d59c160072145869ca74f23541b3a2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 01 Oct 2021 22:42:38 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Tue, 02 Nov 2021 21:29:08 GMT
ADD file:8a77a81970b6a702c1b54fad57fad996bfa087b741913c5e6497f56f8e4189cb in / 
# Tue, 02 Nov 2021 21:29:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e90ab5cf9c8733234d970ca9a967d31286943996a9eb293f507785641cc7e149`  
		Last Modified: Tue, 02 Nov 2021 21:30:21 GMT  
		Size: 55.2 MB (55158170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
