<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:0208464c31d28e57a01193119e933cdb3bab417b1b148f2481162b74a49c12f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:a40ac480314b234ba17c1a5feba12ae96961adcc0ffdae316fa508271d1d22cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88103710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08fe7e10e646d0eaf1cbb06d153d72f668e4054d65b632751c581dc374f4cef7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 09 May 2022 18:23:04 GMT
ADD file:ca9e196ff03d648b77dda6c48467c5f9f9fb6ca722caeb5c80255f3d19f1085a in / 
# Mon, 09 May 2022 18:23:05 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 09 May 2022 18:23:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1e0c3a1cbe1453559314c935bc256e5087a0a4ac5b88f65ee3d9275c1bd901c0`  
		Last Modified: Mon, 09 May 2022 18:23:25 GMT  
		Size: 88.1 MB (88103493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a40718f6834d24f0bdeddee666030fabca745fe9088d98926b8c63ada205953`  
		Last Modified: Mon, 09 May 2022 18:23:13 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:0208464c31d28e57a01193119e933cdb3bab417b1b148f2481162b74a49c12f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:a40ac480314b234ba17c1a5feba12ae96961adcc0ffdae316fa508271d1d22cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88103710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08fe7e10e646d0eaf1cbb06d153d72f668e4054d65b632751c581dc374f4cef7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 09 May 2022 18:23:04 GMT
ADD file:ca9e196ff03d648b77dda6c48467c5f9f9fb6ca722caeb5c80255f3d19f1085a in / 
# Mon, 09 May 2022 18:23:05 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 09 May 2022 18:23:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1e0c3a1cbe1453559314c935bc256e5087a0a4ac5b88f65ee3d9275c1bd901c0`  
		Last Modified: Mon, 09 May 2022 18:23:25 GMT  
		Size: 88.1 MB (88103493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a40718f6834d24f0bdeddee666030fabca745fe9088d98926b8c63ada205953`  
		Last Modified: Mon, 09 May 2022 18:23:13 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
