## `photon:latest`

```console
$ docker pull photon@sha256:9785fc642d79e7d2f89ab82c289098b7e40383d86a54f85b8f6475598b627c57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:b1081f4cf496aa8cef1d9f7e1e96ba094c99fa9b5a29830038b9295c4b54ee15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15131493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf8e3dfef5c248bc8880d228241887a1f411b0d2700150e3eeb6ad8c5763df2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 04 Feb 2020 01:21:32 GMT
ADD file:009c0128bda1df8f213f8d4029d839550798c744c86621b575e9db7f4eb32b17 in / 
# Tue, 04 Feb 2020 01:21:32 GMT
LABEL name=Photon OS x86_64/3.0 Base Image vendor=VMware build-date=20200202
# Tue, 04 Feb 2020 01:21:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:663010993c44c37a1efaeeba4ed0f9904a6a7ce39d97f5ba5026760e314cade6`  
		Last Modified: Tue, 04 Feb 2020 01:22:12 GMT  
		Size: 15.1 MB (15131493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:027b8c2c1e898d8f35ebe0a5334c43ba4efb1ff25e7cb5468c55f21f6f18b6be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12940485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf50306275906cb0fa05c1c76656950e7c6ff86867cca37bd7b3370395c8c43`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 04 Feb 2020 01:45:32 GMT
ADD file:7ce77ac1cea7a8ad86c19f91e34759c30c7a8d54bca7097e590c0127593d4cfe in / 
# Tue, 04 Feb 2020 01:45:34 GMT
LABEL name=Photon OS aarch64/3.0 Base Image vendor=VMware build-date=20200202
# Tue, 04 Feb 2020 01:45:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6e59bcd05047d8b229a221c54b98960a2ab57309a19cef0daa179dae63b8bde5`  
		Last Modified: Tue, 04 Feb 2020 01:45:52 GMT  
		Size: 12.9 MB (12940485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
