## `oraclelinux:8-slim`

```console
$ docker pull oraclelinux@sha256:d440054c384a78ee5affeff69b8acac3f9e375e8249b10b946c9eb31bba004a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `oraclelinux:8-slim` - linux; amd64

```console
$ docker pull oraclelinux@sha256:8a15bc9084b2c23b01802e9db71195cf0c1eca057a3cc4e4e0426fd883392cac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54163019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b030151f96aa5e29a50148504640b2905d7c592faf8fe984a7184d7fe62081f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Sep 2020 21:22:07 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 30 Oct 2020 02:05:51 GMT
ADD file:ca74b6a4572ba9ecd7ceca8360a2d15560bf779277672ae9a37e25c53f8d1226 in / 
# Fri, 30 Oct 2020 02:05:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9f8aeb516aa1b01143452930dec1cadef36b4298bcdb43224755b12ab4bc9289`  
		Last Modified: Fri, 30 Oct 2020 02:07:57 GMT  
		Size: 54.2 MB (54163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `oraclelinux:8-slim` - linux; arm64 variant v8

```console
$ docker pull oraclelinux@sha256:0703e8b3b5cc0ba1c9573f2c9a83e55af553e4a99f964c94a8a0dd4243c97a78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54285957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f068c78e9933158db296551172fb7e8c495f6e39053ca52794702c25f74452`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Sep 2020 20:40:54 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 22 Oct 2020 02:02:57 GMT
ADD file:91f94052d144e7fac61501c6d72e663eda67c40303d29f0b62fda4abe0e5a284 in / 
# Thu, 22 Oct 2020 02:03:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:428aa11a26cf7698a25c3ec8f290dd1667191a70a5797b7232fa597f1e52ec1b`  
		Last Modified: Thu, 22 Oct 2020 02:04:59 GMT  
		Size: 54.3 MB (54285957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
