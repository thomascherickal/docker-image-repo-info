## `photon:latest`

```console
$ docker pull photon@sha256:5816a5831b44cbbca7793a132e9d74962d8df8b3c2d238c92c039ed0fe6d6364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:37e9cd932ff0bbf08649dac04488e80ac527f275bda0bd5d5eb080a4e77d6654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15795455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34772bc276e610fd7531ddfbccbefbf1283e81c07a0f5d74d4f45baa6b24305e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Jun 2021 21:54:13 GMT
ADD file:38190c17be8564316840af747b4b73d1923bc602bcaa9e3d07af1cbbe30a99cc in / 
# Tue, 22 Jun 2021 21:54:13 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20210621
# Tue, 22 Jun 2021 21:54:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:08318d195c4bd32d4b683471a1317e52acc790eefe3d397b3a64e935fc15fe7d`  
		Last Modified: Tue, 22 Jun 2021 21:55:02 GMT  
		Size: 15.8 MB (15795455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:78331b9ffd6eac6db4b7610dc19bc8b5f9dc15076ee534f54c4db008163d87fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14949126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af9109c4e639828064813cc7053c808a04e29e63d96abd936e50045f081dd3fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 26 Jun 2021 02:25:54 GMT
ADD file:ba66c3814a075f729f3cbcb8823d4530cae4bb2a504a27db0b9bf7c777b03178 in / 
# Sat, 26 Jun 2021 02:25:54 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20210625
# Sat, 26 Jun 2021 02:25:55 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9817f3f8002f1b6160a96dd2fc56907cae92f957ae310d327b8f753b8b8b4176`  
		Last Modified: Sat, 26 Jun 2021 02:26:25 GMT  
		Size: 14.9 MB (14949126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
