## `photon:latest`

```console
$ docker pull photon@sha256:5ab660bcc9e233089894221151fb0985cf0e944db83d31ef93783ed24dd7ba09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:441f3c28b653bce8a19e4a0213fd071a540f7897d70b5c7c7e01aef6a52357a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15923220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058e730fd5932431dd80cb643a1d13036b5cd6256c8b94a643ff8019da42027f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 21 Aug 2023 19:27:36 GMT
ADD file:9efd366f27570f4bfe9509739b33dbf32904d9675cb99ef1f5148d8575d7c1d7 in / 
# Mon, 21 Aug 2023 19:27:37 GMT
LABEL name=Photon OS x86_64/5.0 Base Image vendor=VMware build-date=20230819
# Mon, 21 Aug 2023 19:27:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e8a5cf3bb1101a15782997d005b52cda87a92e316c70f6dee1ecd25b2b3915fd`  
		Last Modified: Mon, 21 Aug 2023 19:28:01 GMT  
		Size: 15.9 MB (15923220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:a51ab1e240df3a7a1390a225aa0c2f0aee422b96dc95bd1d60f2615850e63263
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14929499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece71ad42c3f7f2aa11531d8b0f7b36dc226ae2a927e10d75f66b471f4e8b170`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 28 Aug 2023 20:27:14 GMT
ADD file:f2b6eb3fc1c93853dc60d29b62e2de6c76a0f71b28db68392a656b10d4ddcf17 in / 
# Mon, 28 Aug 2023 20:27:15 GMT
LABEL name=Photon OS aarch64/5.0 Base Image vendor=VMware build-date=20230826
# Mon, 28 Aug 2023 20:27:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0fbf17b4b6de782f8c9924a2b1a2b466db7e2b97f190563ec327f8cb3f2f1717`  
		Last Modified: Mon, 28 Aug 2023 20:27:35 GMT  
		Size: 14.9 MB (14929499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
