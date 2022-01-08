## `photon:latest`

```console
$ docker pull photon@sha256:5c2857aadb8be1464b502e655c1b9c72ee375de020581a8e755c04f063d7ad96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:9ec7b54b5b21bd1cf7c88d0108d508a4d16eebf1ca7a987e58de8f5c990b95b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16808791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684eca7e619fe20790204b65063bcdb01237bbddd0265407173c183506b1047e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 08 Jan 2022 02:20:59 GMT
ADD file:713ab0578effcf32095e0b421898496cad85a2033db52ddf2b33003f2c580a03 in / 
# Sat, 08 Jan 2022 02:20:59 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20220107
# Sat, 08 Jan 2022 02:21:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e28db5caeae73c6f8c8434d5f56042f1e9c33e70ffa008bc47e01d04fd163602`  
		Last Modified: Sat, 08 Jan 2022 02:21:45 GMT  
		Size: 16.8 MB (16808791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:9bf00bd3181f28354e873ed2e8ab63996129e2aabd94d537814fe6e597921bcc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15815057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0986a49df4eade98404b1b651c4bedb9ed530a54b8dea37e0c486c29a0c6a450`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 08 Jan 2022 02:49:28 GMT
ADD file:40aa333e6c6dc420ee4b85e9832f32735eeaab1f02e747c78cb18fb227ddcc73 in / 
# Sat, 08 Jan 2022 02:49:28 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20220107
# Sat, 08 Jan 2022 02:49:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b71733efd441f1db107d778f12dab04b97070fc2ff6d8bf255200740743bd15c`  
		Last Modified: Sat, 08 Jan 2022 02:49:57 GMT  
		Size: 15.8 MB (15815057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
