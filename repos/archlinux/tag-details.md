<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20221211.0.109768`](#archlinuxbase-202212110109768)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20221211.0.109768`](#archlinuxbase-devel-202212110109768)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:2eb5372d8e6d6a16575b7483544cecb9b5bb35f654594c75e3c84838b5db7544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:e98008b351bf47ada7efe158b9220d403cd555d86353b5d457b53e72bd7ef727
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141809154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50279e9f2546fe76fff3e18897010bc2cbb188ad9a62bc260c8cb683a118767b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Dec 2022 20:19:51 GMT
COPY dir:48ab6d1ef10204fcea7f0fe1fb1fb0c1d03aae627091060cf59340b5f88981e3 in / 
# Mon, 12 Dec 2022 20:19:52 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 12 Dec 2022 20:19:53 GMT
ENV LANG=C.UTF-8
# Mon, 12 Dec 2022 20:19:53 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:ff1caeb8e1af152c988a72c6f36e3221dac74b60f089ec8f71651119697eba01`  
		Last Modified: Mon, 12 Dec 2022 20:21:35 GMT  
		Size: 141.8 MB (141801185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505b4dbbb765e6af8ccfc37d0997d638797774082251dfc66084f1d12fb3958b`  
		Last Modified: Mon, 12 Dec 2022 20:21:15 GMT  
		Size: 8.0 KB (7969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20221211.0.109768`

```console
$ docker pull archlinux@sha256:2eb5372d8e6d6a16575b7483544cecb9b5bb35f654594c75e3c84838b5db7544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20221211.0.109768` - linux; amd64

```console
$ docker pull archlinux@sha256:e98008b351bf47ada7efe158b9220d403cd555d86353b5d457b53e72bd7ef727
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141809154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50279e9f2546fe76fff3e18897010bc2cbb188ad9a62bc260c8cb683a118767b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Dec 2022 20:19:51 GMT
COPY dir:48ab6d1ef10204fcea7f0fe1fb1fb0c1d03aae627091060cf59340b5f88981e3 in / 
# Mon, 12 Dec 2022 20:19:52 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 12 Dec 2022 20:19:53 GMT
ENV LANG=C.UTF-8
# Mon, 12 Dec 2022 20:19:53 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:ff1caeb8e1af152c988a72c6f36e3221dac74b60f089ec8f71651119697eba01`  
		Last Modified: Mon, 12 Dec 2022 20:21:35 GMT  
		Size: 141.8 MB (141801185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505b4dbbb765e6af8ccfc37d0997d638797774082251dfc66084f1d12fb3958b`  
		Last Modified: Mon, 12 Dec 2022 20:21:15 GMT  
		Size: 8.0 KB (7969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:c8b95aeb80103e3b23e5bd2a9a95da17aae97033bac7ea3ffa81aab9ddeb70d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:6a69ef51b378b54267e0a586dd3e8a08f88de2089349dc33497e15468151c29b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.0 MB (243031321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c2cd56ad0967ab0c7c63933a26b3536ac44367c3070f7fac01c6eca94dacfa`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Dec 2022 20:20:51 GMT
COPY dir:5cd2e889b898a10ff0b003cf6eeb987182554f44af4ea277b44647d1a2061a73 in / 
# Mon, 12 Dec 2022 20:20:54 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 12 Dec 2022 20:20:54 GMT
ENV LANG=C.UTF-8
# Mon, 12 Dec 2022 20:20:54 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:2bdca0923c12cab704a400d8e21a44209994395f7e48d32f2b4e6a5124eb877e`  
		Last Modified: Mon, 12 Dec 2022 20:22:21 GMT  
		Size: 243.0 MB (243022693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff276260fe9975fd9db874ad88b53a8c37ca5a4f46d040319df6dc983f9c1937`  
		Last Modified: Mon, 12 Dec 2022 20:21:46 GMT  
		Size: 8.6 KB (8628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20221211.0.109768`

```console
$ docker pull archlinux@sha256:c8b95aeb80103e3b23e5bd2a9a95da17aae97033bac7ea3ffa81aab9ddeb70d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20221211.0.109768` - linux; amd64

```console
$ docker pull archlinux@sha256:6a69ef51b378b54267e0a586dd3e8a08f88de2089349dc33497e15468151c29b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.0 MB (243031321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c2cd56ad0967ab0c7c63933a26b3536ac44367c3070f7fac01c6eca94dacfa`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Dec 2022 20:20:51 GMT
COPY dir:5cd2e889b898a10ff0b003cf6eeb987182554f44af4ea277b44647d1a2061a73 in / 
# Mon, 12 Dec 2022 20:20:54 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 12 Dec 2022 20:20:54 GMT
ENV LANG=C.UTF-8
# Mon, 12 Dec 2022 20:20:54 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:2bdca0923c12cab704a400d8e21a44209994395f7e48d32f2b4e6a5124eb877e`  
		Last Modified: Mon, 12 Dec 2022 20:22:21 GMT  
		Size: 243.0 MB (243022693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff276260fe9975fd9db874ad88b53a8c37ca5a4f46d040319df6dc983f9c1937`  
		Last Modified: Mon, 12 Dec 2022 20:21:46 GMT  
		Size: 8.6 KB (8628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:2eb5372d8e6d6a16575b7483544cecb9b5bb35f654594c75e3c84838b5db7544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:e98008b351bf47ada7efe158b9220d403cd555d86353b5d457b53e72bd7ef727
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141809154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50279e9f2546fe76fff3e18897010bc2cbb188ad9a62bc260c8cb683a118767b`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 12 Dec 2022 20:19:51 GMT
COPY dir:48ab6d1ef10204fcea7f0fe1fb1fb0c1d03aae627091060cf59340b5f88981e3 in / 
# Mon, 12 Dec 2022 20:19:52 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 12 Dec 2022 20:19:53 GMT
ENV LANG=C.UTF-8
# Mon, 12 Dec 2022 20:19:53 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:ff1caeb8e1af152c988a72c6f36e3221dac74b60f089ec8f71651119697eba01`  
		Last Modified: Mon, 12 Dec 2022 20:21:35 GMT  
		Size: 141.8 MB (141801185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505b4dbbb765e6af8ccfc37d0997d638797774082251dfc66084f1d12fb3958b`  
		Last Modified: Mon, 12 Dec 2022 20:21:15 GMT  
		Size: 8.0 KB (7969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
