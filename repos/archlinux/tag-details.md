<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20221106.0.100148`](#archlinuxbase-202211060100148)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20221106.0.100148`](#archlinuxbase-devel-202211060100148)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:833f706a0b193fe369ff2e1905ef901b2f57a5c0eb3f9ad09906ac1451b10efe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:3439fd2e47062799f0adb531d3c6e8c24595b1cb047a9db22838e2da56608361
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140621118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e8963f74642d9c68b7402d6ff116534023053ce7b95b1f07d52830d26e4725`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 31 Oct 2022 19:21:16 GMT
COPY dir:945f7f153f8ae3f123f3c78221e7b782f2598f753a8ad7ecd7a9fbd6a780ad87 in / 
# Mon, 31 Oct 2022 19:21:18 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 31 Oct 2022 19:21:18 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2022 19:21:18 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:7d6ea839295cf23eca99481519835740f8619f84dfb047228cfa77d6269194b1`  
		Last Modified: Mon, 31 Oct 2022 19:23:02 GMT  
		Size: 140.6 MB (140613172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9415a322dc16d913bde3128810006517afe9b6c43b6f8d56544372a283132492`  
		Last Modified: Mon, 31 Oct 2022 19:22:41 GMT  
		Size: 7.9 KB (7946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20221106.0.100148`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:8e91ae3cdf71607b3fb3bf68987ea02c36689e8c7a9c6c5c775bf4c9cafa0d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:0d5c4d8c67ff0d0e6fc1300622f0ade7d2d64737a15f3d7a1868257872a0485e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238895820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ad726a254e4b793c77093f7a2e6361d6a74f4dba3022a1db15914835e9bf78`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 31 Oct 2022 19:22:18 GMT
COPY dir:a025c87a1f4f0e296ce35569b702641010c23b46dd748a108a7b067629f0c3c6 in / 
# Mon, 31 Oct 2022 19:22:21 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 31 Oct 2022 19:22:21 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2022 19:22:21 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:37e5c2addda4602ab7cd53c40ebe6fae9e0da05020d21e2560ce3f5ffbe13612`  
		Last Modified: Mon, 31 Oct 2022 19:23:49 GMT  
		Size: 238.9 MB (238887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28dbae0cf3b9eabc35e3c1aa80bd21cd5d91715125fda9018d14bf80c81320a`  
		Last Modified: Mon, 31 Oct 2022 19:23:14 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20221106.0.100148`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:833f706a0b193fe369ff2e1905ef901b2f57a5c0eb3f9ad09906ac1451b10efe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:3439fd2e47062799f0adb531d3c6e8c24595b1cb047a9db22838e2da56608361
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140621118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e8963f74642d9c68b7402d6ff116534023053ce7b95b1f07d52830d26e4725`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 31 Oct 2022 19:21:16 GMT
COPY dir:945f7f153f8ae3f123f3c78221e7b782f2598f753a8ad7ecd7a9fbd6a780ad87 in / 
# Mon, 31 Oct 2022 19:21:18 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 31 Oct 2022 19:21:18 GMT
ENV LANG=C.UTF-8
# Mon, 31 Oct 2022 19:21:18 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:7d6ea839295cf23eca99481519835740f8619f84dfb047228cfa77d6269194b1`  
		Last Modified: Mon, 31 Oct 2022 19:23:02 GMT  
		Size: 140.6 MB (140613172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9415a322dc16d913bde3128810006517afe9b6c43b6f8d56544372a283132492`  
		Last Modified: Mon, 31 Oct 2022 19:22:41 GMT  
		Size: 7.9 KB (7946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
