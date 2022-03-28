<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:496c2548c709c974a66c894a1924951c561cd0834ff17bd6f80b35a9397a7b94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:6690cd7f16f7cdb5130324224f58556ce81d97db6438f8df6fc6e6a692636b8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88063375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9a6d3c7ad8524e102c346396471646626ba5065f2594ccfe267623807486b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 28 Mar 2022 18:19:32 GMT
ADD file:9c03a5b8bca9a07efca13ece3f992e0d7d461de08c70599bf7810b1c2fbac06b in / 
# Mon, 28 Mar 2022 18:19:33 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 28 Mar 2022 18:19:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9c01f1ca7ccb3b15db20473da273d550ed416c8cedfdd90d57e29aa44eb0ae17`  
		Last Modified: Mon, 28 Mar 2022 18:19:56 GMT  
		Size: 88.1 MB (88063157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad7e0127cf12344bd54f017af809a15001f509c079a566afd2195f98dd82332`  
		Last Modified: Mon, 28 Mar 2022 18:19:44 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:496c2548c709c974a66c894a1924951c561cd0834ff17bd6f80b35a9397a7b94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:6690cd7f16f7cdb5130324224f58556ce81d97db6438f8df6fc6e6a692636b8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88063375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9a6d3c7ad8524e102c346396471646626ba5065f2594ccfe267623807486b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 28 Mar 2022 18:19:32 GMT
ADD file:9c03a5b8bca9a07efca13ece3f992e0d7d461de08c70599bf7810b1c2fbac06b in / 
# Mon, 28 Mar 2022 18:19:33 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 28 Mar 2022 18:19:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9c01f1ca7ccb3b15db20473da273d550ed416c8cedfdd90d57e29aa44eb0ae17`  
		Last Modified: Mon, 28 Mar 2022 18:19:56 GMT  
		Size: 88.1 MB (88063157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad7e0127cf12344bd54f017af809a15001f509c079a566afd2195f98dd82332`  
		Last Modified: Mon, 28 Mar 2022 18:19:44 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
