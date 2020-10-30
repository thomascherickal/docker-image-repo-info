## `oraclelinux:7-slim`

```console
$ docker pull oraclelinux@sha256:bc574a4cdb83591874e5c6ce5d9fa468494575d4b1ffc01c30809f8116d1858f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `oraclelinux:7-slim` - linux; amd64

```console
$ docker pull oraclelinux@sha256:0edb15f2df59b86269b264870a027ee1a3835ef95f8d3445b0e4364a53aef32b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48259572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc7e50513559e9783921d59bc71fbd303f831258776bd77463ed27f2920bab4f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 30 Oct 2020 02:06:29 GMT
ADD file:145961aa92d5a9c6b87e124b38a59e7a4a08910f8cb21414300096f88cc5cb82 in / 
# Fri, 30 Oct 2020 02:06:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0df82e2779b8235d6babd25457b87762ea8300fb3797ea03adccf472e7a598df`  
		Last Modified: Fri, 30 Oct 2020 02:08:45 GMT  
		Size: 48.3 MB (48259572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `oraclelinux:7-slim` - linux; arm64 variant v8

```console
$ docker pull oraclelinux@sha256:e53e6498633229abad7b41c698fe115c94e8822d8b524f61cb407801bb4bdb25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48850724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ef754f6859a0f5b4f16e1ebc6810d5bc6e0d417af2b5d379c474b3c430d5a14`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 30 Oct 2020 03:45:28 GMT
ADD file:d06b128d722861d60588554a964338fbb9b6dfcc296d33a7a42703a049cd88b5 in / 
# Fri, 30 Oct 2020 03:45:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:52c09b6ca87b8b24b91cb6a8012a6e48a4a855b5a01f8a6076a66f42e7be2fc8`  
		Last Modified: Fri, 30 Oct 2020 03:47:43 GMT  
		Size: 48.9 MB (48850724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
