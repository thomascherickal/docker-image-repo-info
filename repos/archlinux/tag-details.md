<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230305.0.131236`](#archlinuxbase-202303050131236)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230305.0.131236`](#archlinuxbase-devel-202303050131236)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:30365f3f73505e0ef43b91981a6a5cd95c5d62494458117157cdf36ee0e78267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:a65f53f97982062eadc297a145b6d4fbb7e59dfd61e1cec0e906435741595c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142248323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99ae5175e028d2a534a76f7af729d0f50fa5be4fcd7233e09bc5a1dcc753990d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 06 Mar 2023 20:20:06 GMT
COPY dir:fb86575c29a95c41862e97a810a71a359414ece74fbbacbaaaa83aa57811007a in / 
# Mon, 06 Mar 2023 20:20:08 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 06 Mar 2023 20:20:08 GMT
ENV LANG=C.UTF-8
# Mon, 06 Mar 2023 20:20:08 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f13ce42b43249e06dbc68212e727fb44794adcf8a88d2351fba0101c01a7b929`  
		Last Modified: Mon, 06 Mar 2023 20:21:39 GMT  
		Size: 142.2 MB (142240383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e62cddd826166f44ecdc4776ec30cf2cf75dd8b564658436a102ce7478d335`  
		Last Modified: Mon, 06 Mar 2023 20:21:19 GMT  
		Size: 7.9 KB (7940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230305.0.131236`

```console
$ docker pull archlinux@sha256:30365f3f73505e0ef43b91981a6a5cd95c5d62494458117157cdf36ee0e78267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20230305.0.131236` - linux; amd64

```console
$ docker pull archlinux@sha256:a65f53f97982062eadc297a145b6d4fbb7e59dfd61e1cec0e906435741595c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142248323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99ae5175e028d2a534a76f7af729d0f50fa5be4fcd7233e09bc5a1dcc753990d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 06 Mar 2023 20:20:06 GMT
COPY dir:fb86575c29a95c41862e97a810a71a359414ece74fbbacbaaaa83aa57811007a in / 
# Mon, 06 Mar 2023 20:20:08 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 06 Mar 2023 20:20:08 GMT
ENV LANG=C.UTF-8
# Mon, 06 Mar 2023 20:20:08 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f13ce42b43249e06dbc68212e727fb44794adcf8a88d2351fba0101c01a7b929`  
		Last Modified: Mon, 06 Mar 2023 20:21:39 GMT  
		Size: 142.2 MB (142240383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e62cddd826166f44ecdc4776ec30cf2cf75dd8b564658436a102ce7478d335`  
		Last Modified: Mon, 06 Mar 2023 20:21:19 GMT  
		Size: 7.9 KB (7940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:da2cfd0975150f4fa2091141e6362e9630e0bb8fb20840c47fd6fa9bf0f0122b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:9988f99b27c40c82c00ff138c9541d3bbbb8d05bfbe678211c5a6923a4e84772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.2 MB (245230845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97342c4da63f8760b15bb7ad2028f7ede20591bdff0d1048974e6ec8f202f7bc`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 06 Mar 2023 20:21:05 GMT
COPY dir:85e801d5104e24925c4ba0a585ff1227475b04c7885fc0d6a7b36658158629f6 in / 
# Mon, 06 Mar 2023 20:21:09 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 06 Mar 2023 20:21:09 GMT
ENV LANG=C.UTF-8
# Mon, 06 Mar 2023 20:21:09 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:6df10e147b58b3665928d52d81decc4a5f82594edb43f401e10cdc3f33b8e778`  
		Last Modified: Mon, 06 Mar 2023 20:22:24 GMT  
		Size: 245.2 MB (245222117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a5e71ef32dcb7dbb34eb6268fc2fa886886227cd4a7f461151e750440b8c7b`  
		Last Modified: Mon, 06 Mar 2023 20:21:49 GMT  
		Size: 8.7 KB (8728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230305.0.131236`

```console
$ docker pull archlinux@sha256:da2cfd0975150f4fa2091141e6362e9630e0bb8fb20840c47fd6fa9bf0f0122b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230305.0.131236` - linux; amd64

```console
$ docker pull archlinux@sha256:9988f99b27c40c82c00ff138c9541d3bbbb8d05bfbe678211c5a6923a4e84772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.2 MB (245230845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97342c4da63f8760b15bb7ad2028f7ede20591bdff0d1048974e6ec8f202f7bc`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 06 Mar 2023 20:21:05 GMT
COPY dir:85e801d5104e24925c4ba0a585ff1227475b04c7885fc0d6a7b36658158629f6 in / 
# Mon, 06 Mar 2023 20:21:09 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 06 Mar 2023 20:21:09 GMT
ENV LANG=C.UTF-8
# Mon, 06 Mar 2023 20:21:09 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:6df10e147b58b3665928d52d81decc4a5f82594edb43f401e10cdc3f33b8e778`  
		Last Modified: Mon, 06 Mar 2023 20:22:24 GMT  
		Size: 245.2 MB (245222117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a5e71ef32dcb7dbb34eb6268fc2fa886886227cd4a7f461151e750440b8c7b`  
		Last Modified: Mon, 06 Mar 2023 20:21:49 GMT  
		Size: 8.7 KB (8728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:30365f3f73505e0ef43b91981a6a5cd95c5d62494458117157cdf36ee0e78267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:a65f53f97982062eadc297a145b6d4fbb7e59dfd61e1cec0e906435741595c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142248323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99ae5175e028d2a534a76f7af729d0f50fa5be4fcd7233e09bc5a1dcc753990d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 06 Mar 2023 20:20:06 GMT
COPY dir:fb86575c29a95c41862e97a810a71a359414ece74fbbacbaaaa83aa57811007a in / 
# Mon, 06 Mar 2023 20:20:08 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 06 Mar 2023 20:20:08 GMT
ENV LANG=C.UTF-8
# Mon, 06 Mar 2023 20:20:08 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f13ce42b43249e06dbc68212e727fb44794adcf8a88d2351fba0101c01a7b929`  
		Last Modified: Mon, 06 Mar 2023 20:21:39 GMT  
		Size: 142.2 MB (142240383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e62cddd826166f44ecdc4776ec30cf2cf75dd8b564658436a102ce7478d335`  
		Last Modified: Mon, 06 Mar 2023 20:21:19 GMT  
		Size: 7.9 KB (7940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
