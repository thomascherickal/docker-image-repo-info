## `photon:latest`

```console
$ docker pull photon@sha256:97c26d1aa0fc9571b437bc1e19bf7445ccde795b8d7ce10d2e600163aef73ff4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:ba6a5e0592483f28827545ce100f711aa602adf100e5884840c56c5b9b059acc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15153321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3697a7ed6ddafe1d21609016de9780344f79504879a2153cdb2de81466f58e27`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 17 Apr 2020 20:23:11 GMT
ADD file:8977940c5bfd0be1e27cac9394290b34ce29c9a16b1e9be164e5e93ba4cb403c in / 
# Fri, 17 Apr 2020 20:23:11 GMT
LABEL name=Photon OS x86_64/3.0 Base Image vendor=VMware build-date=20200417
# Fri, 17 Apr 2020 20:23:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3478fd58133b768140e03314353a1d1bd854ae7cbfdebdd26a02742129edb8c3`  
		Last Modified: Fri, 17 Apr 2020 20:23:29 GMT  
		Size: 15.2 MB (15153321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:25d76ab105865deada5693c228e56ae5fc3c282c2e7af25e07fb779b0871cc0b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12949841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7602766763e2993fbd81e1e8da47d317edb8a7383eff03991ac43d76689d12f3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Apr 2020 19:40:44 GMT
ADD file:8883f2695673a13bdfcbe86568fd7f6b73b5fbf862943f65a9f9534e29bce790 in / 
# Mon, 06 Apr 2020 19:40:45 GMT
LABEL name=Photon OS aarch64/3.0 Base Image vendor=VMware build-date=20200403
# Mon, 06 Apr 2020 19:40:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c0269f537c11928477a816177a5e6ffcec23d786f6a27cde4f691fd50e7296b7`  
		Last Modified: Mon, 06 Apr 2020 19:40:59 GMT  
		Size: 12.9 MB (12949841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
