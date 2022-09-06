<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20220904.0.80503`](#archlinuxbase-20220904080503)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20220904.0.80503`](#archlinuxbase-devel-20220904080503)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:3b698b409dcb528682d337b872e0b463753885e8adf246dc4d1b15ea3ec3ff15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:c979e393ff728b75a709ce2b302cfc60844bfca7c5195f35ba6f70bdc06ccb8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138529611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546c416f6b9d42e11beab7b426a422f88b4d6de9b1edcc68a431764b42be64d5`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 06 Sep 2022 22:19:50 GMT
COPY dir:80fa47a9aaca5e3bc65671bb68f78fabda8df2578c24de2b2957512ba16c2a4a in / 
# Tue, 06 Sep 2022 22:19:52 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 06 Sep 2022 22:19:52 GMT
ENV LANG=C.UTF-8
# Tue, 06 Sep 2022 22:19:52 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:285486683dddc0a5fe5a7c38ea2310b4cbd30810102b95602819509ec11f08c6`  
		Last Modified: Tue, 06 Sep 2022 22:21:57 GMT  
		Size: 138.5 MB (138521523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb2109147fbd15f1668df981a020317738cdac87741a320c0bf604180096c10`  
		Last Modified: Tue, 06 Sep 2022 22:21:14 GMT  
		Size: 8.1 KB (8088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20220904.0.80503`

```console
$ docker pull archlinux@sha256:3b698b409dcb528682d337b872e0b463753885e8adf246dc4d1b15ea3ec3ff15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20220904.0.80503` - linux; amd64

```console
$ docker pull archlinux@sha256:c979e393ff728b75a709ce2b302cfc60844bfca7c5195f35ba6f70bdc06ccb8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138529611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546c416f6b9d42e11beab7b426a422f88b4d6de9b1edcc68a431764b42be64d5`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 06 Sep 2022 22:19:50 GMT
COPY dir:80fa47a9aaca5e3bc65671bb68f78fabda8df2578c24de2b2957512ba16c2a4a in / 
# Tue, 06 Sep 2022 22:19:52 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 06 Sep 2022 22:19:52 GMT
ENV LANG=C.UTF-8
# Tue, 06 Sep 2022 22:19:52 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:285486683dddc0a5fe5a7c38ea2310b4cbd30810102b95602819509ec11f08c6`  
		Last Modified: Tue, 06 Sep 2022 22:21:57 GMT  
		Size: 138.5 MB (138521523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb2109147fbd15f1668df981a020317738cdac87741a320c0bf604180096c10`  
		Last Modified: Tue, 06 Sep 2022 22:21:14 GMT  
		Size: 8.1 KB (8088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:bff528014b2611b1222c2a2e1ceb1284bb6771e17bb03fc7e6a182bcdfc58ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:a999a6f345c5103f9ce411847e1936239c47898d3fe94d98ef001077c4ee9911
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236785254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a01d94e04f5aee0a99f9cc6d7444f6f7d601e1664f0ee191ffd3a25358366df`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 06 Sep 2022 22:20:52 GMT
COPY dir:db8a5bb926f70f4d8949676c07b91b42fb2eb2cee8533c0985579e8aaadccc14 in / 
# Tue, 06 Sep 2022 22:20:55 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 06 Sep 2022 22:20:55 GMT
ENV LANG=C.UTF-8
# Tue, 06 Sep 2022 22:20:55 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:869ff801500f2793d5c539409a49cf7d1638f246c26f02cd5c43862a7489fe71`  
		Last Modified: Tue, 06 Sep 2022 22:22:45 GMT  
		Size: 236.8 MB (236776485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1d836123b5bf29996b66aa80febf87d2403926490375a059a63f3c6063fb99`  
		Last Modified: Tue, 06 Sep 2022 22:22:09 GMT  
		Size: 8.8 KB (8769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20220904.0.80503`

```console
$ docker pull archlinux@sha256:bff528014b2611b1222c2a2e1ceb1284bb6771e17bb03fc7e6a182bcdfc58ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220904.0.80503` - linux; amd64

```console
$ docker pull archlinux@sha256:a999a6f345c5103f9ce411847e1936239c47898d3fe94d98ef001077c4ee9911
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236785254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a01d94e04f5aee0a99f9cc6d7444f6f7d601e1664f0ee191ffd3a25358366df`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 06 Sep 2022 22:20:52 GMT
COPY dir:db8a5bb926f70f4d8949676c07b91b42fb2eb2cee8533c0985579e8aaadccc14 in / 
# Tue, 06 Sep 2022 22:20:55 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 06 Sep 2022 22:20:55 GMT
ENV LANG=C.UTF-8
# Tue, 06 Sep 2022 22:20:55 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:869ff801500f2793d5c539409a49cf7d1638f246c26f02cd5c43862a7489fe71`  
		Last Modified: Tue, 06 Sep 2022 22:22:45 GMT  
		Size: 236.8 MB (236776485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1d836123b5bf29996b66aa80febf87d2403926490375a059a63f3c6063fb99`  
		Last Modified: Tue, 06 Sep 2022 22:22:09 GMT  
		Size: 8.8 KB (8769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:3b698b409dcb528682d337b872e0b463753885e8adf246dc4d1b15ea3ec3ff15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:c979e393ff728b75a709ce2b302cfc60844bfca7c5195f35ba6f70bdc06ccb8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138529611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546c416f6b9d42e11beab7b426a422f88b4d6de9b1edcc68a431764b42be64d5`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 06 Sep 2022 22:19:50 GMT
COPY dir:80fa47a9aaca5e3bc65671bb68f78fabda8df2578c24de2b2957512ba16c2a4a in / 
# Tue, 06 Sep 2022 22:19:52 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 06 Sep 2022 22:19:52 GMT
ENV LANG=C.UTF-8
# Tue, 06 Sep 2022 22:19:52 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:285486683dddc0a5fe5a7c38ea2310b4cbd30810102b95602819509ec11f08c6`  
		Last Modified: Tue, 06 Sep 2022 22:21:57 GMT  
		Size: 138.5 MB (138521523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb2109147fbd15f1668df981a020317738cdac87741a320c0bf604180096c10`  
		Last Modified: Tue, 06 Sep 2022 22:21:14 GMT  
		Size: 8.1 KB (8088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
