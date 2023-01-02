<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230101.0.115167`](#archlinuxbase-202301010115167)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230101.0.115167`](#archlinuxbase-devel-202301010115167)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:69fdc54a81d49999287f54b5b2432e9c9237270fc28a0139114f57933b17945a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:37dbbfa36f6e5834d00f91d63fc202d20daf9b91d3f5a09a24121f7564331a76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141883033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d0c96df6f809dbe10416a632f084976e91cbfc92e58f8c856dac70f99c92c6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:19:54 GMT
COPY dir:3abf814353e83b9530d12b2ee4cb160eb0fb2ee78d0d92a5f66dff25261b5897 in / 
# Mon, 02 Jan 2023 18:19:56 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 02 Jan 2023 18:19:56 GMT
ENV LANG=C.UTF-8
# Mon, 02 Jan 2023 18:19:56 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b72d4d4e6198ff7d4f89d0158a130599ce521e31e57fdf9eb55f74654d6e440b`  
		Last Modified: Mon, 02 Jan 2023 18:21:39 GMT  
		Size: 141.9 MB (141875088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b001a57ac96ef2bbff38f455389cad90c31da42bdb7a74e3ab5cf0071f36444`  
		Last Modified: Mon, 02 Jan 2023 18:21:18 GMT  
		Size: 7.9 KB (7945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230101.0.115167`

```console
$ docker pull archlinux@sha256:69fdc54a81d49999287f54b5b2432e9c9237270fc28a0139114f57933b17945a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20230101.0.115167` - linux; amd64

```console
$ docker pull archlinux@sha256:37dbbfa36f6e5834d00f91d63fc202d20daf9b91d3f5a09a24121f7564331a76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141883033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d0c96df6f809dbe10416a632f084976e91cbfc92e58f8c856dac70f99c92c6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:19:54 GMT
COPY dir:3abf814353e83b9530d12b2ee4cb160eb0fb2ee78d0d92a5f66dff25261b5897 in / 
# Mon, 02 Jan 2023 18:19:56 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 02 Jan 2023 18:19:56 GMT
ENV LANG=C.UTF-8
# Mon, 02 Jan 2023 18:19:56 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b72d4d4e6198ff7d4f89d0158a130599ce521e31e57fdf9eb55f74654d6e440b`  
		Last Modified: Mon, 02 Jan 2023 18:21:39 GMT  
		Size: 141.9 MB (141875088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b001a57ac96ef2bbff38f455389cad90c31da42bdb7a74e3ab5cf0071f36444`  
		Last Modified: Mon, 02 Jan 2023 18:21:18 GMT  
		Size: 7.9 KB (7945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:20f1ad0d1e75fcfd8b541de0f519d343430f30cb3f963b5adc8676c6091dd407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:3a64011140ee44f1c11c62abdb0426b04791db4c342e7d092932ca9a583e75b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.2 MB (243227812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2e09c7919211f6c26a8aa57ca8aba7cd99ec53002b959087ac9581ce8dc7be`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:20:54 GMT
COPY dir:677ff053e258db1091a13c2e0d19dfb63a89c574c24c57260b5b72921ec06ee8 in / 
# Mon, 02 Jan 2023 18:20:57 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 02 Jan 2023 18:20:57 GMT
ENV LANG=C.UTF-8
# Mon, 02 Jan 2023 18:20:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:62eaba580f07c2f8b6125f83da13ef8687865016ba06a46064202023afdf74f8`  
		Last Modified: Mon, 02 Jan 2023 18:22:25 GMT  
		Size: 243.2 MB (243219199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76e32eee8a9098df21fcc9166844129c4afc058df8515af76a22738c5829177`  
		Last Modified: Mon, 02 Jan 2023 18:21:49 GMT  
		Size: 8.6 KB (8613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230101.0.115167`

```console
$ docker pull archlinux@sha256:20f1ad0d1e75fcfd8b541de0f519d343430f30cb3f963b5adc8676c6091dd407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230101.0.115167` - linux; amd64

```console
$ docker pull archlinux@sha256:3a64011140ee44f1c11c62abdb0426b04791db4c342e7d092932ca9a583e75b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.2 MB (243227812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2e09c7919211f6c26a8aa57ca8aba7cd99ec53002b959087ac9581ce8dc7be`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:20:54 GMT
COPY dir:677ff053e258db1091a13c2e0d19dfb63a89c574c24c57260b5b72921ec06ee8 in / 
# Mon, 02 Jan 2023 18:20:57 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 02 Jan 2023 18:20:57 GMT
ENV LANG=C.UTF-8
# Mon, 02 Jan 2023 18:20:58 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:62eaba580f07c2f8b6125f83da13ef8687865016ba06a46064202023afdf74f8`  
		Last Modified: Mon, 02 Jan 2023 18:22:25 GMT  
		Size: 243.2 MB (243219199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76e32eee8a9098df21fcc9166844129c4afc058df8515af76a22738c5829177`  
		Last Modified: Mon, 02 Jan 2023 18:21:49 GMT  
		Size: 8.6 KB (8613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:69fdc54a81d49999287f54b5b2432e9c9237270fc28a0139114f57933b17945a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:37dbbfa36f6e5834d00f91d63fc202d20daf9b91d3f5a09a24121f7564331a76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141883033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d0c96df6f809dbe10416a632f084976e91cbfc92e58f8c856dac70f99c92c6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:19:54 GMT
COPY dir:3abf814353e83b9530d12b2ee4cb160eb0fb2ee78d0d92a5f66dff25261b5897 in / 
# Mon, 02 Jan 2023 18:19:56 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 02 Jan 2023 18:19:56 GMT
ENV LANG=C.UTF-8
# Mon, 02 Jan 2023 18:19:56 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b72d4d4e6198ff7d4f89d0158a130599ce521e31e57fdf9eb55f74654d6e440b`  
		Last Modified: Mon, 02 Jan 2023 18:21:39 GMT  
		Size: 141.9 MB (141875088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b001a57ac96ef2bbff38f455389cad90c31da42bdb7a74e3ab5cf0071f36444`  
		Last Modified: Mon, 02 Jan 2023 18:21:18 GMT  
		Size: 7.9 KB (7945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
