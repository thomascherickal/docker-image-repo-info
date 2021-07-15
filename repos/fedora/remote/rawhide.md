## `fedora:rawhide`

```console
$ docker pull fedora@sha256:cee477106e31dec61a6c9c7b78ef38ce8e3e68d4ecdc296e17a0740460f8b81c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:8d75dfe0c04eead604d648c43227387bba254bbf1aadd196c6b613ce16198b55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65056928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a66a425e85bce0b4bd0c2c4546fdee7a1e9ee33a73bf865877d8fdb53b00cc8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 01 Apr 2021 18:00:32 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Fri, 14 May 2021 17:21:09 GMT
ADD file:c3b28974735ca99c48d05a9f6d4da52a54fd658b1ec0752f59f5ff6e0dccf779 in / 
# Fri, 14 May 2021 17:21:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:963ac42671b20a7712e5fe7316fd3faca6fca23b8c774275c437ff8523201ea4`  
		Last Modified: Fri, 14 May 2021 17:22:18 GMT  
		Size: 65.1 MB (65056928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm variant v7

```console
$ docker pull fedora@sha256:279d803e0177d111651f4c1df8f9d13937f86754b280dde1313ec0b4c127e99b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61600385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5967044dea83fcdbf2c70c3d0a3d442307c49d4417c2fe4ad00cb603f260ef43`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 09 Oct 2020 21:02:51 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 27 Apr 2021 22:07:26 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Fri, 14 May 2021 18:08:11 GMT
ADD file:06a02d8e54ae19996acba8216b88e209db85dad847445978b239f52fa666af73 in / 
# Fri, 14 May 2021 18:08:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3150253f8ad0abee250b2a1e43725995e804484296b6894fa4ee872d11cfea1d`  
		Last Modified: Fri, 14 May 2021 18:10:03 GMT  
		Size: 61.6 MB (61600385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:cd50a4d12fd6d6b147f1cd3bdb693d815bd009c31a0b733b19c33765cdc46927
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64975390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9937ba3cef82884f847dfee39b16a56f8236179ad47bfafd91b819bdb066a56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Mon, 25 Jan 2021 23:41:07 GMT
ENV DISTTAG=fRawhidecontainer FGC=fRawhide FBR=fRawhide
# Fri, 14 May 2021 17:58:07 GMT
ADD file:90e79766eaf14910faff056a09dbc292acc85c847a2a2f304f562b8b426ae47c in / 
# Fri, 14 May 2021 17:58:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a71b5fc8949eeedcda33224323758dd4a4b804b64d574ac2d199f8ebefe79b1`  
		Last Modified: Fri, 14 May 2021 17:59:31 GMT  
		Size: 65.0 MB (64975390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
