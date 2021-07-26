## `archlinux:base`

```console
$ docker pull archlinux@sha256:339ce5aad19cb7bb40cfbb171504fca2622fef754282ceb8f945b60b2fb7b728
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:4f8a53da4df161a89502c436de35f466dfa33950bc635564c45cb8e548590566
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134833427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd558cc83192dcf791c12f1c2bcc638fc80455cf9cf104443f5b2ff70dd369ab`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 26 Jul 2021 18:23:32 GMT
COPY dir:dce2c6b75525659521502720c37eb3f195315190905ce6bb6400a1da49749c80 in / 
# Mon, 26 Jul 2021 18:23:34 GMT
RUN ldconfig
# Mon, 26 Jul 2021 18:23:34 GMT
ENV LANG=en_US.UTF-8
# Mon, 26 Jul 2021 18:23:34 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f286e38b7f70947665c0615115f8356a2b92d48475bcb801ad8578dff68d1c4b`  
		Last Modified: Mon, 26 Jul 2021 18:25:17 GMT  
		Size: 134.8 MB (134826766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccbbafc02d18d0613a7db30c35e6b098488903bf48da69941bb79a65861e1cd`  
		Last Modified: Mon, 26 Jul 2021 18:24:58 GMT  
		Size: 6.7 KB (6661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
