## `fedora:latest`

```console
$ docker pull fedora@sha256:790a32ab1f4d0efc8ca9027d75bc54ba70edd3babd3897655760af8ba837637f
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
$ docker pull fedora@sha256:486fd5578f93fbc57a519e34ad4b7cac927c3f8a95409baedf0c19e9f287c207
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58926165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ffdbffd20736862c8955419ef7db69849d715131717697007c3e51f22915a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:00 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 12 May 2022 18:22:54 GMT
ADD file:58865512ca3855cdfdc2144a71fb60de2340fdef4a00331a533d5c76abd5bf01 in / 
# Thu, 12 May 2022 18:22:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e1deda52ffad5c9c8e3b7151625b679af50d6459630f4bf0fbf49e161dba4e88`  
		Last Modified: Thu, 12 May 2022 18:23:31 GMT  
		Size: 58.9 MB (58926165 bytes)  
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
$ docker pull fedora@sha256:f149778a36890280d9052e56ae7be6a50484c4c3828c68c692415849d3519b9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (57016241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8847e9bf6df80d7720e7daa5788671263f03a108a19cff8ff8c6f5f17fcad348`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 02 Nov 2021 21:12:33 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 19:19:40 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 12 May 2022 18:42:58 GMT
ADD file:0ee69bd7b31ad9a58ac1e11f1dca4f03039f993866babfd024c92101871a0696 in / 
# Thu, 12 May 2022 18:42:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9d693e29d403003707f47a0a8d2d7d4909e9407adfd64496ca4b67afead1bb2a`  
		Last Modified: Thu, 12 May 2022 18:43:42 GMT  
		Size: 57.0 MB (57016241 bytes)  
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
$ docker pull fedora@sha256:a4a89ebb890dae892d8ba8c241a487fa91d07a26231055b7ecda408aa1c8811c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55866395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1185b4b6acae3561cf2cb14466fa70d0290abaf7f6cfa1c61cf9d7ac427bec16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 04:31:33 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 12 May 2022 18:43:32 GMT
ADD file:e8ee7a53af42a85aab0b35476966872f3783deb8471e0a8608272329a1a4a443 in / 
# Thu, 12 May 2022 18:43:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a89d4a56299d6e7abd0e5c76dfaf3d48e4d8f9141a7e23cf6ae832aae4bad2aa`  
		Last Modified: Thu, 12 May 2022 18:44:23 GMT  
		Size: 55.9 MB (55866395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
