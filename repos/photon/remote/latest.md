## `photon:latest`

```console
$ docker pull photon@sha256:62b0ae4870071ff6dbcd5534e169b832b813440c738444b014b4540042c44a2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:150eeb984e1a8d4332111d0e5aca6e8c3934389c1aedf824b2455be2eccd3abe
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15134003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d1c0daff50faed20e3dde5026f9696a22930debb43776ce366d8ac10199959`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 25 Jan 2020 02:31:27 GMT
ADD file:c28d12250324c29b40ac649d93443c99484e8580895d59e0ec643ff30cea2065 in / 
# Sat, 25 Jan 2020 02:31:27 GMT
LABEL name=Photon OS x86_64/3.0 Base Image vendor=VMware build-date=20200124
# Sat, 25 Jan 2020 02:31:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:39bdb4c1af72822e587799601caf585b2dc8cd492dab0007e201cae3367feece`  
		Last Modified: Sat, 25 Jan 2020 02:32:15 GMT  
		Size: 15.1 MB (15134003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:42b8f3373cb8603c5ff72c44096b0c54f0d4fa33719b09b381450ae82026934e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12951279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:279cbdf5941e8db93ab05d4457a2523c05cf920b2f283f08edad394f1e10b94b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 25 Jan 2020 02:05:04 GMT
ADD file:5b2c22237afa0b7d7d4538da2db0fa2d05c05a9c0b73e3ba31430d1e28b70bfc in / 
# Sat, 25 Jan 2020 02:05:07 GMT
LABEL name=Photon OS aarch64/3.0 Base Image vendor=VMware build-date=20200124
# Sat, 25 Jan 2020 02:05:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:347103b036d0d857ad734e0c109c06c871b118daf6f10f9f94ea4a2128c374ef`  
		Last Modified: Sat, 25 Jan 2020 02:05:31 GMT  
		Size: 13.0 MB (12951279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
