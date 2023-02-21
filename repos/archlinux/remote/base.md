## `archlinux:base`

```console
$ docker pull archlinux@sha256:5cc161b8a1d493717ee1f607e0f0350675b13f7f2b87a6108c8fc7c74249b859
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:51b107accb235f48045a76a8edfbd642b0552901a15d12b31ce9dc837ae7c116
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142199312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4a2f4b224566e3a0f1f12d242476477060056de119ae93bedd0a104055b3284`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 21 Feb 2023 20:20:29 GMT
COPY dir:55040eda790f0fb66f5b2ff97c2b4ab73ad4971aed159c268247c6b94dd84903 in / 
# Tue, 21 Feb 2023 20:20:31 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 21 Feb 2023 20:20:31 GMT
ENV LANG=C.UTF-8
# Tue, 21 Feb 2023 20:20:31 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:09ad74402c61846b4ee53a70c13d18de68b4f14097aab33f00fc2340dfb569ee`  
		Last Modified: Tue, 21 Feb 2023 20:22:15 GMT  
		Size: 142.2 MB (142191355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b9eb5ca00dbba9f4fa45f05d16dc708fbbb5564567095e608ed3f7f0ab562e`  
		Last Modified: Tue, 21 Feb 2023 20:21:56 GMT  
		Size: 8.0 KB (7957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
