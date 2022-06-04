## `photon:latest`

```console
$ docker pull photon@sha256:60b0e97c4b39639e69cde20af3d32b46f895ad7aeb2b68657446af4bc754db01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:5910d46076c74f08327c6c6c2d25a7321921d2cb6ededc0ec4f08d7a5d933c72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15994577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a211faa08363be35086ee466c1e5c9d464d312f5b523abad3db417839f6dacf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 03 Jun 2022 23:20:04 GMT
ADD file:d3f5520a9ad28f5cf073f013103b0b5837f2a14bf5b7cee03e6fb78c66153135 in / 
# Fri, 03 Jun 2022 23:20:04 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20220603
# Fri, 03 Jun 2022 23:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cb54d1184a86b82843c849bbd232f27fd0b1b012c8770baea97b5a05244b2f48`  
		Last Modified: Fri, 03 Jun 2022 23:20:35 GMT  
		Size: 16.0 MB (15994577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:50f64c72bb36a480786d9a09353105e15e29ee9deb62d450ef65fb88791148f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15064470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d67e55fb26afe13a537a2d80e23b87964ab334dd383f08d636047833c6660c55`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 03 Jun 2022 23:40:18 GMT
ADD file:ecbad7d26310f4def7098fa578c4338d220bfb598de4eb1efc30f4ccbb038434 in / 
# Fri, 03 Jun 2022 23:40:18 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20220603
# Fri, 03 Jun 2022 23:40:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e6d3e7c5b7cb7de365180f19e27de53e04b67efb294a7d3750fcb7a13556c396`  
		Last Modified: Fri, 03 Jun 2022 23:40:48 GMT  
		Size: 15.1 MB (15064470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
