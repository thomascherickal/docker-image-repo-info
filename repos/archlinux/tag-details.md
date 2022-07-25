<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20220724.0.70393`](#archlinuxbase-20220724070393)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20220724.0.70393`](#archlinuxbase-devel-20220724070393)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:3a527a8a777472e60c23cf7a610b4d082913a786254c002d1cafdcec7f6129d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:241e64d7c13344c931fdaa1ac1712011f4f319b3c616b9bb5da913b17d5cdfdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85959482086fe54cabce80d71f90bb225cd2acd5a86145c5893375c8864935f7`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 25 Jul 2022 18:20:00 GMT
COPY dir:02973f36479d9e568727d88b9c712200b5b259f1b4229152a74889df8abce961 in / 
# Mon, 25 Jul 2022 18:20:01 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 25 Jul 2022 18:20:01 GMT
ENV LANG=C.UTF-8
# Mon, 25 Jul 2022 18:20:01 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8e7389294d1c61bd989a67c9b058aa2c9cedb156cd9640160637ab7ed559377e`  
		Last Modified: Mon, 25 Jul 2022 18:21:45 GMT  
		Size: 127.4 MB (127382407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e306815467656950db37846be1308c3638f406a37c1b59fa9f7f787eddddd77`  
		Last Modified: Mon, 25 Jul 2022 18:21:25 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20220724.0.70393`

```console
$ docker pull archlinux@sha256:3a527a8a777472e60c23cf7a610b4d082913a786254c002d1cafdcec7f6129d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20220724.0.70393` - linux; amd64

```console
$ docker pull archlinux@sha256:241e64d7c13344c931fdaa1ac1712011f4f319b3c616b9bb5da913b17d5cdfdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85959482086fe54cabce80d71f90bb225cd2acd5a86145c5893375c8864935f7`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 25 Jul 2022 18:20:00 GMT
COPY dir:02973f36479d9e568727d88b9c712200b5b259f1b4229152a74889df8abce961 in / 
# Mon, 25 Jul 2022 18:20:01 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 25 Jul 2022 18:20:01 GMT
ENV LANG=C.UTF-8
# Mon, 25 Jul 2022 18:20:01 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8e7389294d1c61bd989a67c9b058aa2c9cedb156cd9640160637ab7ed559377e`  
		Last Modified: Mon, 25 Jul 2022 18:21:45 GMT  
		Size: 127.4 MB (127382407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e306815467656950db37846be1308c3638f406a37c1b59fa9f7f787eddddd77`  
		Last Modified: Mon, 25 Jul 2022 18:21:25 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:ac93e93490a71b30bd8d272ea32071f5380cdc6cf49a8a3fb44b67454b33ce3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:1b89c35fa7e0edc4ed863dc0556a84579bf82e57a5cb4993f2840d7400c09273
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223785056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0472ed96157702bff6dda67efefff6ab38abe7603735ccff692291eeab7d5543`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 25 Jul 2022 18:21:01 GMT
COPY dir:e63c09bfc3564481675b4d0a42923874135b9e688f480a88b73952d1456308b4 in / 
# Mon, 25 Jul 2022 18:21:04 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 25 Jul 2022 18:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 25 Jul 2022 18:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:1b64ff134606a0a90a5a5d9a291a36c4d715d2a0e87a57c916e0245cacf1c079`  
		Last Modified: Mon, 25 Jul 2022 18:22:31 GMT  
		Size: 223.8 MB (223776883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8f2ee8107d38684c0fb84f8613cc7a60b28d73653f0d9aba1caab716baa7f3`  
		Last Modified: Mon, 25 Jul 2022 18:21:56 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20220724.0.70393`

```console
$ docker pull archlinux@sha256:ac93e93490a71b30bd8d272ea32071f5380cdc6cf49a8a3fb44b67454b33ce3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20220724.0.70393` - linux; amd64

```console
$ docker pull archlinux@sha256:1b89c35fa7e0edc4ed863dc0556a84579bf82e57a5cb4993f2840d7400c09273
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223785056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0472ed96157702bff6dda67efefff6ab38abe7603735ccff692291eeab7d5543`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 25 Jul 2022 18:21:01 GMT
COPY dir:e63c09bfc3564481675b4d0a42923874135b9e688f480a88b73952d1456308b4 in / 
# Mon, 25 Jul 2022 18:21:04 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 25 Jul 2022 18:21:04 GMT
ENV LANG=C.UTF-8
# Mon, 25 Jul 2022 18:21:04 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:1b64ff134606a0a90a5a5d9a291a36c4d715d2a0e87a57c916e0245cacf1c079`  
		Last Modified: Mon, 25 Jul 2022 18:22:31 GMT  
		Size: 223.8 MB (223776883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8f2ee8107d38684c0fb84f8613cc7a60b28d73653f0d9aba1caab716baa7f3`  
		Last Modified: Mon, 25 Jul 2022 18:21:56 GMT  
		Size: 8.2 KB (8173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:3a527a8a777472e60c23cf7a610b4d082913a786254c002d1cafdcec7f6129d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:241e64d7c13344c931fdaa1ac1712011f4f319b3c616b9bb5da913b17d5cdfdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85959482086fe54cabce80d71f90bb225cd2acd5a86145c5893375c8864935f7`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 25 Jul 2022 18:20:00 GMT
COPY dir:02973f36479d9e568727d88b9c712200b5b259f1b4229152a74889df8abce961 in / 
# Mon, 25 Jul 2022 18:20:01 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 25 Jul 2022 18:20:01 GMT
ENV LANG=C.UTF-8
# Mon, 25 Jul 2022 18:20:01 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8e7389294d1c61bd989a67c9b058aa2c9cedb156cd9640160637ab7ed559377e`  
		Last Modified: Mon, 25 Jul 2022 18:21:45 GMT  
		Size: 127.4 MB (127382407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e306815467656950db37846be1308c3638f406a37c1b59fa9f7f787eddddd77`  
		Last Modified: Mon, 25 Jul 2022 18:21:25 GMT  
		Size: 7.6 KB (7570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
