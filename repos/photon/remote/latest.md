## `photon:latest`

```console
$ docker pull photon@sha256:8154473f0b361394de4c02e91e20981faed5ac6cb4106203fe5c65ad03be16f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:e333a2c8f3f32f0552ee4a232c8866ab5a18b0ba747d18cbae0162ffc7c2e28a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15178729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20128ff1243a41791c84ed4911d705939dc964eeae60cec28cf362287654851f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 22 Jun 2020 15:20:49 GMT
ADD file:7f35f7ce1d65a169e9215daf9800cb2c17d4398ce9accf81389009a77f09e993 in / 
# Mon, 22 Jun 2020 15:20:49 GMT
LABEL name=Photon OS x86_64/3.0 Base Image vendor=VMware build-date=20200612
# Mon, 22 Jun 2020 15:20:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e6450a72f9eb23edb6d087fe66bd525d229c57e37945f3ceb8511f9aa5241bef`  
		Last Modified: Mon, 22 Jun 2020 15:21:29 GMT  
		Size: 15.2 MB (15178729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:962913600c663fe2db6ecf8579b2f079f428e229de09daa146d4f856cf3c7c51
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12976629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd4a488e1de18b6d7825a4efe55cbbec8bbb1f25bdc7ed7907ee08b406f5dbcc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 22 Jun 2020 15:45:51 GMT
ADD file:08c665f0ba7777994f1048548fdb328043bfbdac97f88d85b1640a7f85dd205c in / 
# Mon, 22 Jun 2020 15:45:53 GMT
LABEL name=Photon OS aarch64/3.0 Base Image vendor=VMware build-date=20200612
# Mon, 22 Jun 2020 15:45:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1b711cdaa3324a89752db1a5ab62e82f43fb9dfdfad05529af5bff18193877de`  
		Last Modified: Mon, 22 Jun 2020 15:46:18 GMT  
		Size: 13.0 MB (12976629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
