## `archlinux:base`

```console
$ docker pull archlinux@sha256:95024c8e97d6ef47c27960263a5c314196feef40a20b1a0c3f0419920492fb0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:d7b0c636c64e5647f6c618fad6171f709e6e142f36b0fa304a74a237f30666c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142323130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e07600b34641f34644e483c95655a9cac108d6e8787f9018e415d58bb0f220`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 20 Mar 2023 23:27:52 GMT
COPY dir:a241af0fc52d72340a9ee4ff7ca91e65eab6a18d07d8680bf1d64e9b317afdfd in / 
# Mon, 20 Mar 2023 23:27:54 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 20 Mar 2023 23:27:54 GMT
ENV LANG=C.UTF-8
# Mon, 20 Mar 2023 23:27:54 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:ef89a47120275cfae011782e1c73d7f57ac5b675c8ec78149ab558c37f8310ff`  
		Last Modified: Mon, 20 Mar 2023 23:29:25 GMT  
		Size: 142.3 MB (142315160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607d5eb3ffd643dd8df0efd9cda3edf68356dfd693886f062bfc8b95da0db656`  
		Last Modified: Mon, 20 Mar 2023 23:29:06 GMT  
		Size: 8.0 KB (7970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
