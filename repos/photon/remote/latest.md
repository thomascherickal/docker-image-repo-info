## `photon:latest`

```console
$ docker pull photon@sha256:259292cf57d6167ebdaf6c5e2b2405b4747289fba7b588e241c40c5ece227478
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:19deea9ff5282c5cddb528966f7ea4597c23ee06c97ef1976b0af2a9f07cb22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16026358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf06d14bcc13554634d9bbcdda51aa429defaa5ddaa85c8e56445e8dd0f8eb5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 30 Jul 2022 00:20:06 GMT
ADD file:709a6fa6ebf8f167e8e3060a3c2f4e1bc67817491517bb50dd01399a57559bc2 in / 
# Sat, 30 Jul 2022 00:20:06 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20220729
# Sat, 30 Jul 2022 00:20:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9fc3011f8f6144788ab6a849f566e66ef4a3d751561602062975c6cef7453cd9`  
		Last Modified: Sat, 30 Jul 2022 00:20:37 GMT  
		Size: 16.0 MB (16026358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:ff658f3c6660b5ca1599ba3aedd14e4b5db0e589928735a9d7adc8d87a3372f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15067806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6e633fe219cc2f704799dd9c2336de5a9a4341dbe6e0dc902eddfc8c640a205`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 22 Jul 2022 22:40:22 GMT
ADD file:223c6fe49d03909b68b17a97236edae180b32a10ba2d1573c5448727e46f8d19 in / 
# Fri, 22 Jul 2022 22:40:22 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20220722
# Fri, 22 Jul 2022 22:40:23 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9ca36a6da01faca896cb368c0a92336889684dc34cd1f106dba5408beedc2b5e`  
		Last Modified: Fri, 22 Jul 2022 22:40:54 GMT  
		Size: 15.1 MB (15067806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
