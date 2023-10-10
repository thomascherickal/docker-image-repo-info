## `photon:latest`

```console
$ docker pull photon@sha256:9dde4a855e8990238fb228b349f90200020d142533279aacdbf32670283e63ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:d89e24728e29b070a1ceef419b8f4ec25032c794b3062f1abfc851ffd5798696
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15940383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e17671b7d250e6bbba09995bb237615ecb9aefe153cfc2e995a81957ca31a7a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 10 Oct 2023 00:20:50 GMT
ADD file:139611ef3734b1b118ff4e8a4ea0c9c705a28d131235ce2bdfeea6512770fefe in / 
# Tue, 10 Oct 2023 00:20:50 GMT
LABEL name=Photon OS x86_64/5.0 Base Image vendor=VMware build-date=20231007
# Tue, 10 Oct 2023 00:20:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7c6c4ff0a1fc7e9ed563a97f5befec547333c628fb380ee88c7e772410ac8fd9`  
		Last Modified: Tue, 10 Oct 2023 00:21:12 GMT  
		Size: 15.9 MB (15940383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:6ee50d1b694bc85a2e394cb915dad2b2d30732bb3c900ebe31f8a3959fffa0be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14941627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c27f4e682f91ec730f3b67e193ee0ab8960a7e744efa8064a3f46798b110f02`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 10 Oct 2023 00:39:51 GMT
ADD file:64c6acd54528667a0e8a0ec1dfd122cb8535909b499489f3afeef726f3376654 in / 
# Tue, 10 Oct 2023 00:39:51 GMT
LABEL name=Photon OS aarch64/5.0 Base Image vendor=VMware build-date=20231007
# Tue, 10 Oct 2023 00:39:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8bec4e3627d62adcfc1576971cc153654f9a21128054886a789444ce8bf24254`  
		Last Modified: Tue, 10 Oct 2023 00:40:05 GMT  
		Size: 14.9 MB (14941627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
