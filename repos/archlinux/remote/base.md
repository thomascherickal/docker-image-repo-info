## `archlinux:base`

```console
$ docker pull archlinux@sha256:979eb993b12e665fcf0c7e454c406ed68e596f3669844f66a56ca859225e7058
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:4a1f1f983df03a1cee7bc7813f79889cd4386c71f8590397d283f925c0a7422d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142242227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff75e574221db7a20bc04e1d20d5d5151b20b30f5ad85f97758859613f92a3b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 13 Mar 2023 20:20:05 GMT
COPY dir:afee26977378a8da2f08119e932279bd8af167ac19027b4b157f1d10cf254fab in / 
# Mon, 13 Mar 2023 20:20:06 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 13 Mar 2023 20:20:06 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 20:20:07 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:d24ecaff127acda26655a6338c1604a6b28e6fd6e8fc8fd33b75437fe51f078e`  
		Last Modified: Mon, 13 Mar 2023 20:21:41 GMT  
		Size: 142.2 MB (142234280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024146e6ccb67f2e2267f1ecc87275ff2283583ac0feab1395bd6fd0abd5c026`  
		Last Modified: Mon, 13 Mar 2023 20:21:22 GMT  
		Size: 7.9 KB (7947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
