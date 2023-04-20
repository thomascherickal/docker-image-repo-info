## `fedora:latest`

```console
$ docker pull fedora@sha256:e1ce95f10501e7c8e3919e33518bf8dea2b8532c80546d1a69774a9810d8b518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:latest` - linux; amd64

```console
$ docker pull fedora@sha256:3f987b7657e944cf87a129cc262982d4f80e38bd98f7db313ccaf90ca7069dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66239195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4c5c8cc5d55e798918c74a615fccb5a0545e99bcf5f2a3891f21305379bac50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:14 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 13 Mar 2023 21:19:47 GMT
ADD file:f5eae77874912e53d0ccece5f455db3cf07ac5e346629ab779ab251c46c0090f in / 
# Mon, 13 Mar 2023 21:19:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:94ee613a6c2156668e36dc8491252e3417ab5be604798abb9e3e469c5e9919e8`  
		Last Modified: Mon, 13 Mar 2023 21:20:48 GMT  
		Size: 66.2 MB (66239195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:85123637b7399d34a2cc410b1fb0d0d3efc0fce39a7d2b6686e7006c341df153
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64445578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2185c9e5402cfe771b816ec39c106860fdc8bf9b1d6cc5c2dff6c77cb8068764`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:31 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 13 Mar 2023 20:39:36 GMT
ADD file:8f1c4c2e60330243e66c553f2377951b11c09601b874f6c778e90ff74c6dc376 in / 
# Mon, 13 Mar 2023 20:39:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e733ff1786fde464ae5c487ee23562295e5ec377f322e1a0ddbeb9eb0b767770`  
		Last Modified: Mon, 13 Mar 2023 20:40:27 GMT  
		Size: 64.4 MB (64445578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; ppc64le

```console
$ docker pull fedora@sha256:ce70b3c02cdff984cfb779fa17f0cc7eac9d5421b411b390760e835d6a3d6eac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71935819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:948fe078f110d54c73abd06b53873031544e7bd673ed7e568a85102de7bae200`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 11 Oct 2022 12:17:51 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 13 Mar 2023 21:17:21 GMT
ADD file:94b146de4812dc44c74e7c714593be878cea336d680f4f5757767c4cf72ece4b in / 
# Mon, 13 Mar 2023 21:17:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8cd4937b22d9f7199d3fc3be560825d6f4c4e2641c0f97e5aebc71924f3d48b4`  
		Last Modified: Mon, 13 Mar 2023 21:19:30 GMT  
		Size: 71.9 MB (71935819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; s390x

```console
$ docker pull fedora@sha256:851ee98c6c36bdff57b0b3dccb45b68cd83cfab3271d90c1c77d305616a6f588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68938038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a6ca8e3ca3f6e473af1a77db6dcee5cc3daff519e8a867277f75a061aa543c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:31:13 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 20 Apr 2023 17:43:33 GMT
ADD file:958dd05dbba98a1bc0862e8829823486b4ea6ad52ebafa192c1dcdbb9431218d in / 
# Thu, 20 Apr 2023 17:43:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f5944babdcdcb1b2a34f534ebc149134fc8caf0879cb2e72b913cdf748b7eacf`  
		Last Modified: Thu, 20 Apr 2023 17:44:40 GMT  
		Size: 68.9 MB (68938038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
