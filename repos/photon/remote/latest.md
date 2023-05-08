## `photon:latest`

```console
$ docker pull photon@sha256:fe84361be8478dc8ecc8a57f4b282cd334ec9fa51f20cb79236a0baf0ab1739a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:66ef3f650de4aeb861c6ab6a139daf5c15e6fecd8988a0a56716dd0c659e6d71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16383637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e402a09f18c32312c8f4845942a570b3ea0701d5643e114a5010235d266048f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 08 May 2023 19:27:50 GMT
ADD file:aa9c2265fcb9ccfca69e0d8a62bf5b2f2c0104e318fffb0dbc25af42365f2b62 in / 
# Mon, 08 May 2023 19:27:50 GMT
LABEL name=Photon OS x86_64/4.0 Base Image vendor=VMware build-date=20230506
# Mon, 08 May 2023 19:27:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fae4a5262fc3293168218e4c43f801ddceb1dfc97a436f7bf7d3bcb8282886a5`  
		Last Modified: Mon, 08 May 2023 19:28:04 GMT  
		Size: 16.4 MB (16383637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:ae913779dc5f9e086f6523df4fa0edfed4f7ab399da840d4d93e22c6e9181810
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15463073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02db826b3c7a3ce554a6ae89fb8351169e686d703a3cb7f66bdbe607b6c928e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 08 May 2023 19:49:21 GMT
ADD file:dafa99bcb2b157e1d5118fb7dddd3aec51f77b591421becbb32c707fdb69ac2f in / 
# Mon, 08 May 2023 19:49:21 GMT
LABEL name=Photon OS aarch64/4.0 Base Image vendor=VMware build-date=20230506
# Mon, 08 May 2023 19:49:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:099d736c15a50669dd5b97eb6af45c26b8e9c1e24b511c3c44de4c0354c17d25`  
		Last Modified: Mon, 08 May 2023 19:49:34 GMT  
		Size: 15.5 MB (15463073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
