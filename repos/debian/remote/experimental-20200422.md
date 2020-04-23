## `debian:experimental-20200422`

```console
$ docker pull debian@sha256:503cf3589e5beb220db30e327bbe784b8fe1b17f0391a2b155e1a2ba0f5ee8b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; mips64le

### `debian:experimental-20200422` - linux; amd64

```console
$ docker pull debian@sha256:22585778342597709836b5e03fca3e64cdc602d0204b8d6dfbcf15d2145e8dd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51979935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598a0c29c569fde1a99fe781d590d72db5706b51d8f510431849666ef988c9be`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:42 GMT
ADD file:6ee109aa41831586899e9a04462a7c3a57fe9b599a263fb0ed2fc3ba1ed57b9b in / 
# Thu, 23 Apr 2020 00:23:43 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:23:58 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1411ff81de269e0758691342315f4c16f9a93db2b77b392e2e3fc3f3ba93b2f1`  
		Last Modified: Thu, 23 Apr 2020 00:28:27 GMT  
		Size: 52.0 MB (51979713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f31581696a65b3d4173140a5bb8db1d74ed3c22a7c834e1eb8b8f4d19dc60ab`  
		Last Modified: Thu, 23 Apr 2020 00:28:40 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200422` - linux; 386

```console
$ docker pull debian@sha256:869b054be7d001857ecdad8f97673228a71efbcabf8e8d598336720272a7ed1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53123934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9822202228ca7c667ce8f0631b1f005460b34212e0e292884ccc74a6e70c8043`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:42:55 GMT
ADD file:1175e5211df616c0061144ef189e0e4972721e25de7304d81f14126234b4bcec in / 
# Thu, 23 Apr 2020 00:42:55 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:43:11 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1831d7d095361283b5fc12083dd3b6702748739d46bc96b030aadf6dfb65f769`  
		Last Modified: Thu, 23 Apr 2020 00:48:31 GMT  
		Size: 53.1 MB (53123709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5550f45d064b7dce5076b86de7c11b525f0ebad9481b0c136a4412e7ddaf8ee5`  
		Last Modified: Thu, 23 Apr 2020 00:48:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200422` - linux; mips64le

```console
$ docker pull debian@sha256:2c5ff7c29542ee3bd0bb1957764f633b50ad05898e1cac66f36f4d4b687a30c9
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50696359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c04cd5f22a1eaf19f4ead327fbb4bb4c70d6aa23248725359498c5b8e1660c59`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:14:06 GMT
ADD file:f4f731cdf85bc353f740a040496bad65f39a579c6a7ee34955a69c0e09ea983b in / 
# Thu, 23 Apr 2020 00:14:07 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:14:31 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5cd8c4531ac615911882437b1e6150cbdcaee37eb6cd1a20c0178acd6b29ab6e`  
		Last Modified: Thu, 23 Apr 2020 00:25:33 GMT  
		Size: 50.7 MB (50696136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13a62aa1f5581f14603946532b9f2ef19ebd8d7536234a2c46950aa957a52b0`  
		Last Modified: Thu, 23 Apr 2020 00:26:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
