## `photon:latest`

```console
$ docker pull photon@sha256:851e2e388f9844e36d03e0ff97ca9bee04f09d9115ec68252b774ba2e5d8a82b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:8bb2d37eaf0ba4afaaa9e42a88200c0016534bf67fca3066a5b35ac91506089b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15975610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b67089cb9bae2d46ea03a2d70447d6829360095cb4e712900462e42db7d9d8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 06 Nov 2021 01:20:10 GMT
ADD file:259675ccf2f14335923f00aa320e7b89935f7f421b0bf33d91bb2937cee6b891 in / 
# Sat, 06 Nov 2021 01:20:11 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20211105
# Sat, 06 Nov 2021 01:20:11 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c931d4b8533835504e204a11235f0530c79d05004ceacfd72a52d1182211d904`  
		Last Modified: Sat, 06 Nov 2021 01:20:46 GMT  
		Size: 16.0 MB (15975610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:f6c688586dbd1e701babdfd6c9b782724b1b09775a84560996c868d09578aee5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15011183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf03042fe34b6917d96a68733102eb1851c9c3c635bc9c27f783a3cdb10ef0b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 06 Nov 2021 00:43:47 GMT
ADD file:bf02ff7235fe3a2024f388308f9f759750cee65040c81d86f8a3a65fb6bb4618 in / 
# Sat, 06 Nov 2021 00:43:47 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20211105
# Sat, 06 Nov 2021 00:43:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:44cbf1f6bba20bd80280d7b4d63c5af59fb58527047f3d0872bcd0d82724ac99`  
		Last Modified: Sat, 06 Nov 2021 00:44:16 GMT  
		Size: 15.0 MB (15011183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
