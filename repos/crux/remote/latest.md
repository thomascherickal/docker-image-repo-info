## `crux:latest`

```console
$ docker pull crux@sha256:afcc4566ea59c522f471da72dcf236ae9d483e21fdc21cb5e02180a1e2aa790d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `crux:latest` - linux; amd64

```console
$ docker pull crux@sha256:b15570468c2dd56d4bd1bd14011b7085d7bcb2179b2d718af235676acd38ddee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159554247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbff4cf50d728c83bd7c2a0b3f966506c40dc1ed3657289eb8cc11d9d1200e0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 21 Nov 2018 16:51:34 GMT
MAINTAINER James Mills, prologic at shortcircuit dot net dot au
# Wed, 16 Sep 2020 17:52:15 GMT
ADD file:9708f8879c5615563d0346084dd67e9b11eb01cea1f187dc42f1b3fea345e8e3 in / 
# Wed, 16 Sep 2020 17:52:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:180a5b3bafc3c941332c0ca2c40e004ae0aabfa7173a28d5ca5f8562f596442a`  
		Last Modified: Wed, 16 Sep 2020 17:55:13 GMT  
		Size: 159.6 MB (159554247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `crux:latest` - linux; arm64 variant v8

```console
$ docker pull crux@sha256:76bb60d03c458c21dfe5f3d21a1bc86fd8643658fab039f4c79570f79ce53acb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141614249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c3f920202f542e2e2a939ae7ed665697f6f370e92a0dad2c456d111e8df108`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Sep 2020 19:03:39 GMT
MAINTAINER James Mills, prologic at shortcircuit dot net dot au
# Wed, 16 Sep 2020 19:03:58 GMT
ADD file:e6680aa5c8d4560a6dbdcf8822a9f578c9767db5918e44b5243b0384154174f1 in / 
# Wed, 16 Sep 2020 19:04:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8e9ae37f73760c07d9368d6028054617dddec7cd95cae2225ce8ff556a4c862f`  
		Last Modified: Wed, 16 Sep 2020 19:05:39 GMT  
		Size: 141.6 MB (141614249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
