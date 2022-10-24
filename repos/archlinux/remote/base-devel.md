## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:421bd2af7f4853edf180cef0b74d8cadfca72c8c92e29bde90fec931a004d91a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:781cbf95c9a6e1331fad7530698c553332f2214d8a90dfc57e917f8f2eeb48ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238885643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:827bc94cc055669ac67a8a8fff40dd7cb074580ce84c4daeb7d8666eef4b970b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 24 Oct 2022 21:21:00 GMT
COPY dir:e2e64ce0c17310fffcad9a034e58b60141f53df9860774b1c80ff4a6af87acae in / 
# Mon, 24 Oct 2022 21:21:03 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 24 Oct 2022 21:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 24 Oct 2022 21:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:9f40941c11469badff128bb105b32a1a5d8e1708e24c266c3ccfae5f1159038f`  
		Last Modified: Mon, 24 Oct 2022 21:22:33 GMT  
		Size: 238.9 MB (238877020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738a92820c5bfe8a40e9f3afb6868e83657adcefffcf51198c605e5d4372ad18`  
		Last Modified: Mon, 24 Oct 2022 21:21:58 GMT  
		Size: 8.6 KB (8623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
