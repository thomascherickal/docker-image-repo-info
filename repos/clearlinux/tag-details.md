<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:0cf821b8d99b9da44a6b38970ad7e22bcf84658ad117cbc5c584cd032154cc9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:103a74e5e97907eb920901b425847f46b26ce31870e72f40f0b1e49f827371e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68066024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e86d8b6bf1e71571142ccb44a8f6485239faa26b90b13da154087448a3be597`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 21 Nov 2023 03:23:47 GMT
ADD file:64fd8d54fcd8cade9e06d346184485e12a7c75bdb9e1c4da1b675732a366a4b9 in / 
# Tue, 21 Nov 2023 03:23:48 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     echo 'root:!:::::::' > /etc/shadow
# Tue, 21 Nov 2023 03:23:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0316dbb764d0f737be1cf2bb682fde8c8d389ba2ef535b1ee80d4aee2c0060a8`  
		Last Modified: Tue, 21 Nov 2023 03:24:05 GMT  
		Size: 68.1 MB (68065810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318e83dbd136e4888734d1eb4353f1ac9c6e16d4c9a06bbae81f7c4e2b3a089e`  
		Last Modified: Tue, 21 Nov 2023 03:23:57 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:0cf821b8d99b9da44a6b38970ad7e22bcf84658ad117cbc5c584cd032154cc9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:103a74e5e97907eb920901b425847f46b26ce31870e72f40f0b1e49f827371e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68066024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e86d8b6bf1e71571142ccb44a8f6485239faa26b90b13da154087448a3be597`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 21 Nov 2023 03:23:47 GMT
ADD file:64fd8d54fcd8cade9e06d346184485e12a7c75bdb9e1c4da1b675732a366a4b9 in / 
# Tue, 21 Nov 2023 03:23:48 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     echo 'root:!:::::::' > /etc/shadow
# Tue, 21 Nov 2023 03:23:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0316dbb764d0f737be1cf2bb682fde8c8d389ba2ef535b1ee80d4aee2c0060a8`  
		Last Modified: Tue, 21 Nov 2023 03:24:05 GMT  
		Size: 68.1 MB (68065810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318e83dbd136e4888734d1eb4353f1ac9c6e16d4c9a06bbae81f7c4e2b3a089e`  
		Last Modified: Tue, 21 Nov 2023 03:23:57 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
