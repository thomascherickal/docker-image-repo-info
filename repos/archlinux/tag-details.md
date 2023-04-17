<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230416.0.143366`](#archlinuxbase-202304160143366)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230416.0.143366`](#archlinuxbase-devel-202304160143366)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:6199cf75da82918db13bbbeef7463e52f1f92b0533187f07632d3676276a64a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:ab2202b76f5c5c4456fba9e5abfe21f2603a488ff341d377eef7baad2bf5582d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143109259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1633d31b65fd7cc20e3990a721222f2e32ac50a3f618c4f941de1682d23b23cf`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 11 Apr 2023 18:19:49 GMT
COPY dir:fd30213caf871300c9eb468a13f832d655779b6531416baa7ba34a5f617b8f5d in / 
# Tue, 11 Apr 2023 18:19:51 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 11 Apr 2023 18:19:51 GMT
ENV LANG=C.UTF-8
# Tue, 11 Apr 2023 18:19:51 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b99db29ebf06f040adbf07770170e673c8ddba414def5cda7e7ec9308085b04b`  
		Last Modified: Tue, 11 Apr 2023 18:21:23 GMT  
		Size: 143.1 MB (143101302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee476ebdd029353b36a23dbf388813dcb17b3d27af5cc7202e881ef32a11938f`  
		Last Modified: Tue, 11 Apr 2023 18:21:04 GMT  
		Size: 8.0 KB (7957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230416.0.143366`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:ad18af22c93d03208f11450638ed59c15d95371589ca1fa0c446602750625cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:8e3e32b6b71897fd55fee0585ac3586e19a65ff94e13792a6b679f1b2fc17a44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.1 MB (246126806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a37dc5345d168f341052800dffb4cb2c2c75acc085b58a492f3473c3a4449586`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 11 Apr 2023 18:20:50 GMT
COPY dir:5e0b9e18a476517bd58f1fad29d1ed47630830094f9d319f506d70cb67034059 in / 
# Tue, 11 Apr 2023 18:20:53 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 11 Apr 2023 18:20:53 GMT
ENV LANG=C.UTF-8
# Tue, 11 Apr 2023 18:20:53 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:f316fb25c719a175ba6a8e01af80a7846c7f563be54a639586fae206ef173d55`  
		Last Modified: Tue, 11 Apr 2023 18:22:07 GMT  
		Size: 246.1 MB (246118099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139b1d0eb0c2028fc2abb922cebc4e3444e9a8e074fae8e6dafe173c4279c716`  
		Last Modified: Tue, 11 Apr 2023 18:21:34 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230416.0.143366`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:6199cf75da82918db13bbbeef7463e52f1f92b0533187f07632d3676276a64a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:ab2202b76f5c5c4456fba9e5abfe21f2603a488ff341d377eef7baad2bf5582d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143109259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1633d31b65fd7cc20e3990a721222f2e32ac50a3f618c4f941de1682d23b23cf`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 11 Apr 2023 18:19:49 GMT
COPY dir:fd30213caf871300c9eb468a13f832d655779b6531416baa7ba34a5f617b8f5d in / 
# Tue, 11 Apr 2023 18:19:51 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 11 Apr 2023 18:19:51 GMT
ENV LANG=C.UTF-8
# Tue, 11 Apr 2023 18:19:51 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:b99db29ebf06f040adbf07770170e673c8ddba414def5cda7e7ec9308085b04b`  
		Last Modified: Tue, 11 Apr 2023 18:21:23 GMT  
		Size: 143.1 MB (143101302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee476ebdd029353b36a23dbf388813dcb17b3d27af5cc7202e881ef32a11938f`  
		Last Modified: Tue, 11 Apr 2023 18:21:04 GMT  
		Size: 8.0 KB (7957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
