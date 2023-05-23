## `photon:latest`

```console
$ docker pull photon@sha256:4d4107666e5e5d37bace6518d49aca36a149ebe3f8febd7b8aa89a3fc19ba9e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:dfb6d68e6c2712bc1c17d5d5b3f12c301121c33fc7154367ba0d35a67563b0df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15908930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d50ac7272e9f5787c582b5703242a60faf109e5b209c89ae9a65d267d0d48e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 May 2023 19:26:40 GMT
ADD file:17ecfeddc8c120d11a3690a8d490132c59cb0932bdee324dff4645fc7f69443a in / 
# Tue, 09 May 2023 19:26:40 GMT
LABEL name=Photon OS x86_64/5.0 Base Image vendor=VMware build-date=20230508
# Tue, 09 May 2023 19:26:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ae34616eeaf007db5f7e646eef1afe9a0c617719ceed1c8d51fbd423759a0a83`  
		Last Modified: Tue, 09 May 2023 19:26:57 GMT  
		Size: 15.9 MB (15908930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:fd412bbcf0ee95048bed9226364f9a257982e24b30d59ce7bd1464fe97aeb040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14908459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6fac23cfc01e0c892555fd0e7c32ddec8849c6bee2efe50fc11e9d15eae694d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 22 May 2023 23:39:47 GMT
ADD file:836bd7f3f0587196613fefb91d5f3c5eb86b732002d523aeb22107b6b0368ba0 in / 
# Mon, 22 May 2023 23:39:47 GMT
LABEL name=Photon OS aarch64/5.0 Base Image vendor=VMware build-date=20230522
# Mon, 22 May 2023 23:39:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:129e4ddda07133e7b6b2b8384d17926879656bfe1df545fe0fc1e02326ae12cb`  
		Last Modified: Mon, 22 May 2023 23:40:03 GMT  
		Size: 14.9 MB (14908459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
