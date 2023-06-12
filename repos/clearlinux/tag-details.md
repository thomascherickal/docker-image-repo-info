<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:83757d20d26fd4da01e129b2e0f46411f14ed0f7bcb9a45a09f521bab4b0dad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:6bb8cbabf11998c94760c79b4d05036dfbec644da6015f5a7c7ce570af4b91cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72607971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c7253045e7d6038a1ea1b3ce81c4f0304565d3ce347dbce7d74db3c184f0d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 12 Jun 2023 18:23:36 GMT
ADD file:7499c241d6a437abc6d2409da1f506f43f7e3d28be02d8f746856c89755a66cf in / 
# Mon, 12 Jun 2023 18:23:37 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 12 Jun 2023 18:23:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e0fe8bc0b8167f63ea13a296a1d5c1f8152283ed49bd93e07702cf1c24834e6d`  
		Last Modified: Mon, 12 Jun 2023 18:23:53 GMT  
		Size: 72.6 MB (72607755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f504ab86b028ac74ac3313f41d97da1dbe2d67883bd5cb1394b15734a21f4b`  
		Last Modified: Mon, 12 Jun 2023 18:23:45 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:83757d20d26fd4da01e129b2e0f46411f14ed0f7bcb9a45a09f521bab4b0dad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:6bb8cbabf11998c94760c79b4d05036dfbec644da6015f5a7c7ce570af4b91cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72607971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c7253045e7d6038a1ea1b3ce81c4f0304565d3ce347dbce7d74db3c184f0d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 12 Jun 2023 18:23:36 GMT
ADD file:7499c241d6a437abc6d2409da1f506f43f7e3d28be02d8f746856c89755a66cf in / 
# Mon, 12 Jun 2023 18:23:37 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 12 Jun 2023 18:23:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e0fe8bc0b8167f63ea13a296a1d5c1f8152283ed49bd93e07702cf1c24834e6d`  
		Last Modified: Mon, 12 Jun 2023 18:23:53 GMT  
		Size: 72.6 MB (72607755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f504ab86b028ac74ac3313f41d97da1dbe2d67883bd5cb1394b15734a21f4b`  
		Last Modified: Mon, 12 Jun 2023 18:23:45 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
