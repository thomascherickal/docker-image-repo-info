<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20230205.0.123931`](#archlinuxbase-202302050123931)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20230205.0.123931`](#archlinuxbase-devel-202302050123931)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:c7b5c89ab205c789d7d4d91732fe9d7f9c361620701dbfd097e2c17e7a961a9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:4501b192ef52888bd0bcaacfa249d6168938d4bfbbfc10ceb60ff047bcc19434
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141907501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f388e052ad9268c81bfccfe5afdaa39ad7e21df4cf9544e8d074eff70b08d2d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 07 Feb 2023 01:21:21 GMT
COPY dir:02cb6e751f7167c871d77dd0f5b9cd13ab96d496d43486d52bafd871a1f1899f in / 
# Tue, 07 Feb 2023 01:21:23 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 07 Feb 2023 01:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:21:23 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4e3865317d3c386d7798f4505406d4f8d80a9bc0ee09f5e93bd13751eab793dc`  
		Last Modified: Tue, 07 Feb 2023 01:23:20 GMT  
		Size: 141.9 MB (141899538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae028eefdd0ebe56ff7949be295fa7c3eed7302a250b38c6904976750d6d97fc`  
		Last Modified: Tue, 07 Feb 2023 01:22:59 GMT  
		Size: 8.0 KB (7963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20230205.0.123931`

```console
$ docker pull archlinux@sha256:c7b5c89ab205c789d7d4d91732fe9d7f9c361620701dbfd097e2c17e7a961a9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-20230205.0.123931` - linux; amd64

```console
$ docker pull archlinux@sha256:4501b192ef52888bd0bcaacfa249d6168938d4bfbbfc10ceb60ff047bcc19434
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141907501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f388e052ad9268c81bfccfe5afdaa39ad7e21df4cf9544e8d074eff70b08d2d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 07 Feb 2023 01:21:21 GMT
COPY dir:02cb6e751f7167c871d77dd0f5b9cd13ab96d496d43486d52bafd871a1f1899f in / 
# Tue, 07 Feb 2023 01:21:23 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 07 Feb 2023 01:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:21:23 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4e3865317d3c386d7798f4505406d4f8d80a9bc0ee09f5e93bd13751eab793dc`  
		Last Modified: Tue, 07 Feb 2023 01:23:20 GMT  
		Size: 141.9 MB (141899538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae028eefdd0ebe56ff7949be295fa7c3eed7302a250b38c6904976750d6d97fc`  
		Last Modified: Tue, 07 Feb 2023 01:22:59 GMT  
		Size: 8.0 KB (7963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:ae4a80a09f6c759676a038fbaebc3f744c0dd23dd01e07b4dd6edfb78a35f237
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:16205ffa58aab2b975467fc59d4acd4f21558da458f54fc535fe37a81806cfba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243487052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c550d9031f67c135c6dd9154a5f2afd924d0b859b4a6f5877c54a7b4de4fa66`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 07 Feb 2023 01:22:38 GMT
COPY dir:9be8ea933917715fc38c864b797a6ce33209be32699cc7148344c74148e398d7 in / 
# Tue, 07 Feb 2023 01:22:42 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 07 Feb 2023 01:22:42 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:22:42 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:fe3c997a2b8a77cf9c9a7a5f8f1dec6d51f9d2330c7e8c73bf0f83681669ba58`  
		Last Modified: Tue, 07 Feb 2023 01:24:07 GMT  
		Size: 243.5 MB (243478410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab90887e196be5bd981c542b642511ab3735e28591beebab9671155c559062c8`  
		Last Modified: Tue, 07 Feb 2023 01:23:31 GMT  
		Size: 8.6 KB (8642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20230205.0.123931`

```console
$ docker pull archlinux@sha256:ae4a80a09f6c759676a038fbaebc3f744c0dd23dd01e07b4dd6edfb78a35f237
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel-20230205.0.123931` - linux; amd64

```console
$ docker pull archlinux@sha256:16205ffa58aab2b975467fc59d4acd4f21558da458f54fc535fe37a81806cfba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243487052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c550d9031f67c135c6dd9154a5f2afd924d0b859b4a6f5877c54a7b4de4fa66`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 07 Feb 2023 01:22:38 GMT
COPY dir:9be8ea933917715fc38c864b797a6ce33209be32699cc7148344c74148e398d7 in / 
# Tue, 07 Feb 2023 01:22:42 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 07 Feb 2023 01:22:42 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:22:42 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:fe3c997a2b8a77cf9c9a7a5f8f1dec6d51f9d2330c7e8c73bf0f83681669ba58`  
		Last Modified: Tue, 07 Feb 2023 01:24:07 GMT  
		Size: 243.5 MB (243478410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab90887e196be5bd981c542b642511ab3735e28591beebab9671155c559062c8`  
		Last Modified: Tue, 07 Feb 2023 01:23:31 GMT  
		Size: 8.6 KB (8642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:c7b5c89ab205c789d7d4d91732fe9d7f9c361620701dbfd097e2c17e7a961a9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:4501b192ef52888bd0bcaacfa249d6168938d4bfbbfc10ceb60ff047bcc19434
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141907501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f388e052ad9268c81bfccfe5afdaa39ad7e21df4cf9544e8d074eff70b08d2d`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 07 Feb 2023 01:21:21 GMT
COPY dir:02cb6e751f7167c871d77dd0f5b9cd13ab96d496d43486d52bafd871a1f1899f in / 
# Tue, 07 Feb 2023 01:21:23 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 07 Feb 2023 01:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 07 Feb 2023 01:21:23 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:4e3865317d3c386d7798f4505406d4f8d80a9bc0ee09f5e93bd13751eab793dc`  
		Last Modified: Tue, 07 Feb 2023 01:23:20 GMT  
		Size: 141.9 MB (141899538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae028eefdd0ebe56ff7949be295fa7c3eed7302a250b38c6904976750d6d97fc`  
		Last Modified: Tue, 07 Feb 2023 01:22:59 GMT  
		Size: 8.0 KB (7963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
