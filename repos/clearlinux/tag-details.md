<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:807adda2af3c0588f37895475685f08560d332f31b9637f50a0c306e0b94e374
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:f7461e25733fde0f313e6c750b660be9cd5afe6ddf78c38850580cfc61ec76d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68044754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2edcfe659e05c52e9cfa66689f8c4e3c25ab0f47eb39bc277432ceec4709d7b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 11 Dec 2023 18:21:13 GMT
ADD file:e0dd020a1b949b3402c42bf7ded6c74fa65dea640188d2de68fbfbc8530b01cd in / 
# Mon, 11 Dec 2023 18:21:14 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     echo 'root:!:::::::' > /etc/shadow
# Mon, 11 Dec 2023 18:21:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9a57e73c07659f03085a2dff7c1ee092c458a33bd5ca086a84d4f2ebbfb4698d`  
		Last Modified: Mon, 11 Dec 2023 18:21:30 GMT  
		Size: 68.0 MB (68044541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b563ccc9f160820a485acac15763e01523e2f84f253ead9981360482958efdb`  
		Last Modified: Mon, 11 Dec 2023 18:21:22 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:807adda2af3c0588f37895475685f08560d332f31b9637f50a0c306e0b94e374
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:f7461e25733fde0f313e6c750b660be9cd5afe6ddf78c38850580cfc61ec76d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68044754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2edcfe659e05c52e9cfa66689f8c4e3c25ab0f47eb39bc277432ceec4709d7b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 11 Dec 2023 18:21:13 GMT
ADD file:e0dd020a1b949b3402c42bf7ded6c74fa65dea640188d2de68fbfbc8530b01cd in / 
# Mon, 11 Dec 2023 18:21:14 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     echo 'root:!:::::::' > /etc/shadow
# Mon, 11 Dec 2023 18:21:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9a57e73c07659f03085a2dff7c1ee092c458a33bd5ca086a84d4f2ebbfb4698d`  
		Last Modified: Mon, 11 Dec 2023 18:21:30 GMT  
		Size: 68.0 MB (68044541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b563ccc9f160820a485acac15763e01523e2f84f253ead9981360482958efdb`  
		Last Modified: Mon, 11 Dec 2023 18:21:22 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
