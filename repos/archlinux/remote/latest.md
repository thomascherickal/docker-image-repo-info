## `archlinux:latest`

```console
$ docker pull archlinux@sha256:52d3c26997e469e9c8ad6221da221f3ce1efe67ed3d6e8088aa1debf66948fd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:02a4c4c4abdcf32e6ebe358409f0a7e66a32afdaca84645a7cdad236e1b7f0db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127278777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e5f5799f5e1d760b6653cdf07fa4932bcd4470c2ffcf15669ceef21d4908be`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 05 Jul 2022 18:19:59 GMT
COPY dir:51ecb096a68d85b3270ed557a4063e9869b4589c5bd483d9ce3bf128d6b55633 in / 
# Tue, 05 Jul 2022 18:20:00 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 05 Jul 2022 18:20:00 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jul 2022 18:20:00 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:fe454d268c1ec66a27de1d34721674ceed43730a84db0fbc8aa90b66b378c234`  
		Last Modified: Tue, 05 Jul 2022 18:21:34 GMT  
		Size: 127.3 MB (127271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890fff2ae0c0183e0f6212c06a4dcaa01be1b03e12814a28149f1094522f5188`  
		Last Modified: Tue, 05 Jul 2022 18:21:15 GMT  
		Size: 7.6 KB (7551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
