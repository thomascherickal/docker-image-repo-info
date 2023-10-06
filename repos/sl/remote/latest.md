## `sl:latest`

```console
$ docker pull sl@sha256:e53124f915798d54be1949a32a88b3f49135ec29eff073cf32217ca83cd30765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sl:latest` - linux; amd64

```console
$ docker pull sl@sha256:d63050e29de7cf9fe5a29996d9d1af345d7ad444b00c2a8a8a52b8ab528e074a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71487075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ac72372bf4ca9f55cecf1b02b45c42252000af0088b5123968ddb558ad609e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 06 Oct 2023 01:42:45 GMT
ADD file:71aaa953562bd3466dd4f76f1e5a5abe3f9c1c78b6a258e3d54f9290c8b65093 in / 
# Fri, 06 Oct 2023 01:42:46 GMT
LABEL name=SL7 Base Image vendor=Scientific Linux build-date=20231005
# Fri, 06 Oct 2023 01:42:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4cd027234441a84bffb7a73ffe5a272f9b31830b6adc6b05111139900738e2b1`  
		Last Modified: Fri, 06 Oct 2023 01:43:03 GMT  
		Size: 71.5 MB (71487075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
