## `photon:latest`

```console
$ docker pull photon@sha256:224588716962a035aba71866e84cbdcf7fe79eed7cb19b9c42d5c29ba2568c4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:9dc3575aa7f0b7f90ba903d1a729626c903766033a7927df6035e136d3c5298b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15915940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d7a3ba8cfd371c1015a87a792e56be5e0fd84764d17c29c6ca1bd4e677780b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jun 2023 21:20:49 GMT
ADD file:5534e22cfb513d4ff9bbf4589d70e2202b93c38a18498b5b8d54116e518d2ce4 in / 
# Mon, 26 Jun 2023 21:20:49 GMT
LABEL name=Photon OS x86_64/5.0 Base Image vendor=VMware build-date=20230624
# Mon, 26 Jun 2023 21:20:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e316eb2a8fe9c65525bb37c570edd1515ae3e4f25d29b4ef7f1e3646d6a4f1c5`  
		Last Modified: Mon, 26 Jun 2023 21:21:12 GMT  
		Size: 15.9 MB (15915940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:58c7dfffe5eac2269c0f8ffa511cf277e2ad7a51416d14062a2fed06cc8549f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14914245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3b94c0976b03b1d8ca311b9997d8cc867f53f90108d19d40e590b242ed5b98`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 26 Jun 2023 21:53:18 GMT
ADD file:15f9763800c2efe923d4764db1068540efb6a717135d675dc5800112e0ac28b4 in / 
# Mon, 26 Jun 2023 21:53:19 GMT
LABEL name=Photon OS aarch64/5.0 Base Image vendor=VMware build-date=20230624
# Mon, 26 Jun 2023 21:53:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:50d45ad74680d6efe320eb7b8676fd68c8427a3569bb347a6ecca0d0ccbdb6c9`  
		Last Modified: Mon, 26 Jun 2023 21:53:38 GMT  
		Size: 14.9 MB (14914245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
