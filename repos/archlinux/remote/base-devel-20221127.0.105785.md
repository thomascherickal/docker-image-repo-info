## `archlinux:base-devel-20221127.0.105785`

```console
$ docker pull archlinux@sha256:e0dc70165b7a0a33a139ffd89896f058fbb8bd433ef7501c625a9df4ac9f8f26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20221127.0.105785` - linux; amd64

```console
$ docker pull archlinux@sha256:5f760fbf6e7eef429b9d10b93b1b596335de7e0f0fdac1d542e5f56676802f5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.1 MB (243063325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab3f933faa07825e0fe9c67836c17a99f71e5597cfcde486fa49b984f0aba762`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 29 Nov 2022 01:20:56 GMT
COPY dir:6ec3d74636391b5514e68cb883db1fe048d9873d4ed1390bb7c78a3fbf0a9b11 in / 
# Tue, 29 Nov 2022 01:20:59 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 29 Nov 2022 01:20:59 GMT
ENV LANG=C.UTF-8
# Tue, 29 Nov 2022 01:20:59 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:9393978b16f1a8e471d3bf5b6e6cefc0be7b98cec824ca2299b7d57ea8aa097f`  
		Last Modified: Tue, 29 Nov 2022 01:22:24 GMT  
		Size: 243.1 MB (243054701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6104f5bc33baa455b2ff0c85077a88ee2f3989298d38b92c16dcca0a477e2afe`  
		Last Modified: Tue, 29 Nov 2022 01:21:49 GMT  
		Size: 8.6 KB (8624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
