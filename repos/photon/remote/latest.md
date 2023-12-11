## `photon:latest`

```console
$ docker pull photon@sha256:8bf91a52bd52466cff011476909578e75d4986b8a7bcf1312ffd7fb64fe63ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:c9c8805e97bf241c193b4d02ea395bc90386cdbba24b8cc7028ade43cf19b85c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15941606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aeaa1c03f1fc9a0ba30a4811a0bdf9c8ff8d6d2398f053a8d9ac9aa56eeca2f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 11 Dec 2023 17:25:40 GMT
ADD file:bb513d988a923796b85c88297959cf60f9bb852a60b0d2f773128fc7786093fd in / 
# Mon, 11 Dec 2023 17:25:40 GMT
LABEL name=Photon OS x86_64/5.0 Base Image vendor=VMware build-date=20231209
# Mon, 11 Dec 2023 17:25:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:577f92c8b679661c141ba125d89658d946290db6b293213f23c90b3b896824b7`  
		Last Modified: Mon, 11 Dec 2023 17:26:23 GMT  
		Size: 15.9 MB (15941606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:399df526b0eb59f34b202ccf94bad317e350d53d1ba712318c85a7d158fb537c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14943772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ac2ef5982af279485f5935e60f965caf2b5bf04646c26f96ebe31fb2964e239`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 23:59:57 GMT
ADD file:13eeb20418509c28c7c216041d2225300b65a19fa82f2733f480882d630d2078 in / 
# Tue, 28 Nov 2023 23:59:57 GMT
LABEL name=Photon OS aarch64/5.0 Base Image vendor=VMware build-date=20231128
# Tue, 28 Nov 2023 23:59:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9eea9d9d1b2af76cb94cefb52bbf2cce46b4f7d30e3bca6b1fae702bc1a3ee45`  
		Last Modified: Wed, 29 Nov 2023 00:00:21 GMT  
		Size: 14.9 MB (14943772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
