<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20221002.0.91257`](#archlinuxbase-20221002091257)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20221002.0.91257`](#archlinuxbase-devel-20221002091257)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:324d260803fa37bc2ff878a17fc13c49cb6352b023b64e58defa9d9fd5fdb792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:3a02e52d5d972230c491b102c3ac586f5299b558b1c501cb181c595e8ba7a40a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140382411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4f097fbe6457d8905a5fb6cfb565c48b34f81a2c7d77479220d80937c17863`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 03 Oct 2022 21:19:56 GMT
COPY dir:357d67580c7d304743f58414e41006932cb5fe247734f1d3ade0e217729b53ca in / 
# Mon, 03 Oct 2022 21:19:58 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 03 Oct 2022 21:19:58 GMT
ENV LANG=C.UTF-8
# Mon, 03 Oct 2022 21:19:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b3230fe6ff2a1bb5ff21943ee7b9b0c441f63a3790bff5954df37f50dfc01ea8`  
		Last Modified: Mon, 03 Oct 2022 21:21:42 GMT  
		Size: 140.4 MB (140374501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b75e13f2371cc7455e28feb7fbaf61bb6c038765c9de103decd343232f5259`  
		Last Modified: Mon, 03 Oct 2022 21:21:22 GMT  
		Size: 7.9 KB (7910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20221002.0.91257`

```console
$ docker pull archlinux@sha256:324d260803fa37bc2ff878a17fc13c49cb6352b023b64e58defa9d9fd5fdb792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20221002.0.91257` - linux; amd64

```console
$ docker pull archlinux@sha256:3a02e52d5d972230c491b102c3ac586f5299b558b1c501cb181c595e8ba7a40a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140382411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4f097fbe6457d8905a5fb6cfb565c48b34f81a2c7d77479220d80937c17863`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 03 Oct 2022 21:19:56 GMT
COPY dir:357d67580c7d304743f58414e41006932cb5fe247734f1d3ade0e217729b53ca in / 
# Mon, 03 Oct 2022 21:19:58 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 03 Oct 2022 21:19:58 GMT
ENV LANG=C.UTF-8
# Mon, 03 Oct 2022 21:19:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b3230fe6ff2a1bb5ff21943ee7b9b0c441f63a3790bff5954df37f50dfc01ea8`  
		Last Modified: Mon, 03 Oct 2022 21:21:42 GMT  
		Size: 140.4 MB (140374501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b75e13f2371cc7455e28feb7fbaf61bb6c038765c9de103decd343232f5259`  
		Last Modified: Mon, 03 Oct 2022 21:21:22 GMT  
		Size: 7.9 KB (7910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:5661abc584c522c46ebf99a12f501703a36fcdfdd9f4953c2cd5b50125abc1dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:2fc3c860b6e61f9759eeaaa4542c429dd8195479da82334bd1509c32fb1886b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238593146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420395b56c93b0fadae42e2f4424e3e4b474ebafd74b486fa59193bd02073f80`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 03 Oct 2022 21:20:58 GMT
COPY dir:18fea0b266ee182d9d39f5c46c96dce2236a702069f997545d0df7b9c4099d49 in / 
# Mon, 03 Oct 2022 21:21:01 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 03 Oct 2022 21:21:01 GMT
ENV LANG=C.UTF-8
# Mon, 03 Oct 2022 21:21:01 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:a64de180eba4662e4ee754ae56002a9e7471e8f9a44f207562a29b6beacd97aa`  
		Last Modified: Mon, 03 Oct 2022 21:22:29 GMT  
		Size: 238.6 MB (238584575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c4e6705d653db25362d4666e5e9cdbec07661b7974c69350629df6a01de0e`  
		Last Modified: Mon, 03 Oct 2022 21:21:54 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20221002.0.91257`

```console
$ docker pull archlinux@sha256:5661abc584c522c46ebf99a12f501703a36fcdfdd9f4953c2cd5b50125abc1dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20221002.0.91257` - linux; amd64

```console
$ docker pull archlinux@sha256:2fc3c860b6e61f9759eeaaa4542c429dd8195479da82334bd1509c32fb1886b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238593146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420395b56c93b0fadae42e2f4424e3e4b474ebafd74b486fa59193bd02073f80`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 03 Oct 2022 21:20:58 GMT
COPY dir:18fea0b266ee182d9d39f5c46c96dce2236a702069f997545d0df7b9c4099d49 in / 
# Mon, 03 Oct 2022 21:21:01 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 03 Oct 2022 21:21:01 GMT
ENV LANG=C.UTF-8
# Mon, 03 Oct 2022 21:21:01 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:a64de180eba4662e4ee754ae56002a9e7471e8f9a44f207562a29b6beacd97aa`  
		Last Modified: Mon, 03 Oct 2022 21:22:29 GMT  
		Size: 238.6 MB (238584575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c4e6705d653db25362d4666e5e9cdbec07661b7974c69350629df6a01de0e`  
		Last Modified: Mon, 03 Oct 2022 21:21:54 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:324d260803fa37bc2ff878a17fc13c49cb6352b023b64e58defa9d9fd5fdb792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:3a02e52d5d972230c491b102c3ac586f5299b558b1c501cb181c595e8ba7a40a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140382411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4f097fbe6457d8905a5fb6cfb565c48b34f81a2c7d77479220d80937c17863`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 03 Oct 2022 21:19:56 GMT
COPY dir:357d67580c7d304743f58414e41006932cb5fe247734f1d3ade0e217729b53ca in / 
# Mon, 03 Oct 2022 21:19:58 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 03 Oct 2022 21:19:58 GMT
ENV LANG=C.UTF-8
# Mon, 03 Oct 2022 21:19:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b3230fe6ff2a1bb5ff21943ee7b9b0c441f63a3790bff5954df37f50dfc01ea8`  
		Last Modified: Mon, 03 Oct 2022 21:21:42 GMT  
		Size: 140.4 MB (140374501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b75e13f2371cc7455e28feb7fbaf61bb6c038765c9de103decd343232f5259`  
		Last Modified: Mon, 03 Oct 2022 21:21:22 GMT  
		Size: 7.9 KB (7910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
