## `oraclelinux:7-slim`

```console
$ docker pull oraclelinux@sha256:e4e9bf19f4dc98bf477b8391465b45a456b7e19dd9025d3dc153a973756f4fd8
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
$ docker pull oraclelinux@sha256:7d3c4670f1fc32bb72cdfa793786d9af97a842734f2bb4b3be22b2e29db400d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48842295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769bef8c512648c67d96d78d3e737d78a82968f3b324fa98ec4e53c47630fb41`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 22 Oct 2020 02:03:38 GMT
ADD file:434be5616fd3939c71e24bfdeef60a8b2ba8daf6f7304554ea178bd308eb21a0 in / 
# Thu, 22 Oct 2020 02:03:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:447d17457bbfc6992a66711a4a20e5492ced489d732f6d943e5a2f8843d8e584`  
		Last Modified: Thu, 22 Oct 2020 02:05:54 GMT  
		Size: 48.8 MB (48842295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
