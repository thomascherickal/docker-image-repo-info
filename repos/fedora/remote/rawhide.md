## `fedora:rawhide`

```console
$ docker pull fedora@sha256:9c4ed23805cf61ff63de92acf1c9e9b9b1b8dfb49c6b2b90f0eaa25363ad5c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:4eeedf5ca28c9f16b33c4a47c435a036dda9c246f2404ca54e190bddc3107c7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63353730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ed9bf0b32c44764a6798766e3fd487d23680d45c3f4d3a915c51a46c0fc762`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Jan 2019 21:21:55 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 25 Aug 2020 18:28:13 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Fri, 02 Oct 2020 21:26:04 GMT
ADD file:44015d20acabdf37f1d46939a84225044cb0a153d7fa41fdd8781adcf850c6a0 in / 
# Fri, 02 Oct 2020 21:26:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:84897672c3cb3bf4d6bb5635513f0ebb6191d0467ce24e2d47b79cf5e5680544`  
		Last Modified: Fri, 02 Oct 2020 21:27:00 GMT  
		Size: 63.4 MB (63353730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:353a341d1c9eba4aeb476e8003a1ea358255971a408901dadc34af15000246ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61541442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c3ff5cf32aaddf9c10daaf33243bd24fca337517949cac7874d7bd15c427690`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 22:43:26 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 25 Aug 2020 17:46:51 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Fri, 02 Oct 2020 20:52:20 GMT
ADD file:4ff63b8f50ba36ad5a8b8fc013219ec831038f2cd06b4759daafd3893e46b58a in / 
# Fri, 02 Oct 2020 20:52:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c19e52334529527cc64041a6ac06de8e2587d5da9193ca1f281840c74cc80063`  
		Last Modified: Fri, 02 Oct 2020 20:53:57 GMT  
		Size: 61.5 MB (61541442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; ppc64le

```console
$ docker pull fedora@sha256:7ab41d92990824647acc87b9b2b3aee8a9b66caec285f1b7d0e16e0679bcfc05
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67135980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da070a0d9ed5ac39f87ea5b6b777aac24f401a5e96a4270782e1044d9477c5a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 05 Jun 2019 23:19:06 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 02 Oct 2020 22:52:10 GMT
ENV DISTTAG=f34container FGC=f34 FBR=f34
# Fri, 02 Oct 2020 22:52:21 GMT
ADD file:bf801fda8043daa26becf13559ff1ee876cb274901ed0480b894d106cce2881c in / 
# Fri, 02 Oct 2020 22:52:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4413bf441c66821b68a5a9975df9eb731a3a5df283cc8512dc26f060b6e71d29`  
		Last Modified: Fri, 02 Oct 2020 22:57:46 GMT  
		Size: 67.1 MB (67135980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
