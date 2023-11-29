<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:494f9bdab2afcbd212eee471f16a5802823d4aa7d6fbbb7c97130cff8e65a7ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:af80534cc6d1e9286073d08766a43ac81e1a83dfca83b2a2b548c30e7552f243
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68058070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a0779ec9b374dd25c9de7156ad2fe74fb9277192f8d6255c081ce9b3ae06ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 28 Nov 2023 23:33:12 GMT
ADD file:811c2a41e312b347f4bbb33217ce8911108c089eb59adca6e1d62aef2eb51f16 in / 
# Tue, 28 Nov 2023 23:33:13 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     echo 'root:!:::::::' > /etc/shadow
# Tue, 28 Nov 2023 23:33:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c64179360a863a3f442ed6e772e50e67543ccda9cf3a2b75cfe2c862977f6d43`  
		Last Modified: Tue, 28 Nov 2023 23:33:38 GMT  
		Size: 68.1 MB (68057857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec931b3c9370d39967c9116e0a0183a38dd58f6df961b62e1afe98e006cbbd6`  
		Last Modified: Tue, 28 Nov 2023 23:33:30 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:494f9bdab2afcbd212eee471f16a5802823d4aa7d6fbbb7c97130cff8e65a7ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:af80534cc6d1e9286073d08766a43ac81e1a83dfca83b2a2b548c30e7552f243
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68058070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a0779ec9b374dd25c9de7156ad2fe74fb9277192f8d6255c081ce9b3ae06ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Tue, 28 Nov 2023 23:33:12 GMT
ADD file:811c2a41e312b347f4bbb33217ce8911108c089eb59adca6e1d62aef2eb51f16 in / 
# Tue, 28 Nov 2023 23:33:13 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     echo 'root:!:::::::' > /etc/shadow
# Tue, 28 Nov 2023 23:33:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c64179360a863a3f442ed6e772e50e67543ccda9cf3a2b75cfe2c862977f6d43`  
		Last Modified: Tue, 28 Nov 2023 23:33:38 GMT  
		Size: 68.1 MB (68057857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec931b3c9370d39967c9116e0a0183a38dd58f6df961b62e1afe98e006cbbd6`  
		Last Modified: Tue, 28 Nov 2023 23:33:30 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
