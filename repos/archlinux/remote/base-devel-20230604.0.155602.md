## `archlinux:base-devel-20230604.0.155602`

```console
$ docker pull archlinux@sha256:a5dafc2b3423f39b4cc9e189710dad87f538d6394c57d74371e342627361bef8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230604.0.155602` - linux; amd64

```console
$ docker pull archlinux@sha256:77a89e28ddcd59e4f6cd74aa144be5596bc22527255c0bb2a50d5396b28e6407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252925084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67ffb784ff04aa8f564e94dca2070164c5415fa13f61a5f132beb6b8296dbe9`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 19:23:42 GMT
COPY dir:83dee47f62aedc3809cee3cb8671c2e3d18eac420969a7d5fa2edf9eed305bf2 in / 
# Mon, 05 Jun 2023 19:23:45 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 05 Jun 2023 19:23:45 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:23:45 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:eb72108021e90da9b83e1a33de6203adf1dc40b5e52134b4330d933755737b63`  
		Last Modified: Mon, 05 Jun 2023 19:24:59 GMT  
		Size: 252.9 MB (252916345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d49bf5cf371455eeb81e9a5b86eb1ca86c1f059caa812b3d68732aa4fbe4e94`  
		Last Modified: Mon, 05 Jun 2023 19:24:25 GMT  
		Size: 8.7 KB (8739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
