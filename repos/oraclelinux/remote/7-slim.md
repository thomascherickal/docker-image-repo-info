## `oraclelinux:7-slim`

```console
$ docker pull oraclelinux@sha256:0a7f2b9b55e63a5a2af918612e2ae1a34e08d022b38138e61f35b6c74b290e96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `oraclelinux:7-slim` - linux; amd64

```console
$ docker pull oraclelinux@sha256:5e0bfb4a9c75dc62119e4ca05d84cdfb2989c02490ac132926aca67ab53383c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48257477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61dfc9a16f3b6375fc6dc7dade077efee1f898475d65219dd3fae0aac6a4a3fb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Wed, 18 Nov 2020 18:16:17 GMT
ADD file:fbc16b85088aeb16b00035f95c6e08678b18cb8a31a4034a171a84b878f95cae in / 
# Wed, 18 Nov 2020 18:16:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:245e9951308ef864ce941f4383344a273da57264b763e6f5aba9347211cf7a40`  
		Last Modified: Wed, 18 Nov 2020 18:17:21 GMT  
		Size: 48.3 MB (48257477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `oraclelinux:7-slim` - linux; arm64 variant v8

```console
$ docker pull oraclelinux@sha256:a6964517b2916b8f1b091f1a97edb63c792c5474a18a07963bb0b25c530da29c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48865698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b424120f0c3a29318d5e8e355efc9b45ce2d3d9b24d74adc983d9850bef6ffe4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 17 Dec 2020 10:54:39 GMT
ADD file:234e637b79d352a87884f78cc7eef7b15ada4bb4afd2ce527325eb690092902f in / 
# Thu, 17 Dec 2020 10:54:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0c52f25eeb980aa519afffa967e1c689524d7fde7d50fc33420a3d54daed23da`  
		Last Modified: Thu, 17 Dec 2020 10:55:54 GMT  
		Size: 48.9 MB (48865698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
