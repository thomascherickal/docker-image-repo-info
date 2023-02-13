## `photon:latest`

```console
$ docker pull photon@sha256:eaacded6efbd97cac525ea7f416381aa03b4c2efeb1b6e1e9961ea65568236f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:8e6f13d05b7170f113bcc821c2e4eed602a3fe930a63c4692e64e92d27aa89f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16081962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c585aef8f81765a10bd52ada54e28f97446c94d428d84874b95623fa08ab47`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 13 Feb 2023 20:26:50 GMT
ADD file:655bdde9587d3b682245c48bac39156bf5a924bd080acac16bdab4325e8d23f8 in / 
# Mon, 13 Feb 2023 20:26:51 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20230211
# Mon, 13 Feb 2023 20:26:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e8f9c57a1510241708a3178d2b0bbb3b8ee61dd4a7010882e49e8df436f91297`  
		Last Modified: Mon, 13 Feb 2023 20:27:14 GMT  
		Size: 16.1 MB (16081962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:3a823aacbaf352771ddea50db09074c1124cd5fe186836ed00adea04e37a7c35
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15168720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60584ed5dfee5062e4850e8be8e143006adf1a4490311569c8e9cfd2d4da9b11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 13 Feb 2023 20:58:27 GMT
ADD file:aefc8b465df0ba7d5685deeeaf1d9d489f0023c098259957f338d103ae7e08e6 in / 
# Mon, 13 Feb 2023 20:58:27 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20230211
# Mon, 13 Feb 2023 20:58:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2cd5d44a3065aefb87ea1614a47dd937989d0b8e3f4ea5fef257ad17135df09a`  
		Last Modified: Mon, 13 Feb 2023 20:58:45 GMT  
		Size: 15.2 MB (15168720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
