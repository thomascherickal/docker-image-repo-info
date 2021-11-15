## `photon:latest`

```console
$ docker pull photon@sha256:08128cee98e8372070fd426adebd98669e42b548f04decd041a48d366500775c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:0cd77cabf6e0b1376c613e0efabdf9a5a7691fdca66b3c14a20446e25e692e4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15975045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7448a40f380db5884994cae3256ee4c94bf9c5a19ea9406c60bb35caee657ffd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 15 Nov 2021 18:20:25 GMT
ADD file:2e1a606debede2b977893e74fff84bd95d28289592326c995a5029cfce2ca0c5 in / 
# Mon, 15 Nov 2021 18:20:25 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20211112
# Mon, 15 Nov 2021 18:20:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7e2a93cf54d6d04e3cb36ae9cd1699d38d6931f82043c1ca4e95bb80f73820f8`  
		Last Modified: Mon, 15 Nov 2021 18:21:11 GMT  
		Size: 16.0 MB (15975045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:44ed712f919cb486d89d8b2dd6c20229d5c2bbc6bb8a604e5157b2f47513af99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15012717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c222761ba8df4ff4e237c56d7bc8c5dffe3a0fbd3a9a1a2989bf716cccff63d5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 15 Nov 2021 18:44:01 GMT
ADD file:31410f88f94f4ba48492f7fdae0a376b4c01e2a5cc971adb80ea9a49c43e4ab9 in / 
# Mon, 15 Nov 2021 18:44:01 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20211112
# Mon, 15 Nov 2021 18:44:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0d10e0b5b4b33835331a202e72dc5fb63c54913c1e095db58f3a6fe071ad13d5`  
		Last Modified: Mon, 15 Nov 2021 18:44:26 GMT  
		Size: 15.0 MB (15012717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
