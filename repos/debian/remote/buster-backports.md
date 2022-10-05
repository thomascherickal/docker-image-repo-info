## `debian:buster-backports`

```console
$ docker pull debian@sha256:49a8985b8c9744503a0d6a60038ae69e957c90ef26a2e16012de8ed5ea88640b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:f5359555419030fe817f5218c9be244d9849213be3c37c10006f8afddd4d6aee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50441324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a512216f10eb4e6c7b7af8f89063df2028139ac5136ac9ca0cacb1e4f5c551c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:50 GMT
ADD file:1fb366429a5df94c7ba642735d6aa77e201f90e0843de03721a6ad19f80ee4e0 in / 
# Tue, 04 Oct 2022 23:26:50 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:26:53 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b6d6a76ebdbe1e858fec4564af6c6c3fe9e9bf1c502c8c8a51afd0fcf3374d44`  
		Last Modified: Tue, 04 Oct 2022 23:31:15 GMT  
		Size: 50.4 MB (50441102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57ff8f54c585a06b90f40c1c1e36c92633f9a7f42d3e71a995ad2d25ca7e01`  
		Last Modified: Tue, 04 Oct 2022 23:31:28 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:afd192c84f2aba8f7ee06140b693db9c7cbe6f19dc7482f1bd101e6cab21a3b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e7e83bcba686568493432a0fa519f5581364f8e3c47df9a27498c9355520f40`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:59:07 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf5f53411b6083b7ee87c4aa7d638953a765cc785c6a28355c28303c35a5e3c`  
		Last Modified: Wed, 05 Oct 2022 00:05:52 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c763c0927ccd28c10a5190b30cb9010c79eee5e676f61247d6c884e8e8ade86f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76f895f7caa5dbd01f30212b687cc5f131c8c5c100825da7aaa75dcc355992f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:45:02 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab18605db3cb6fcd98c199323716b8bbe1f1244dc11eafec4cb4fa6bb1db2034`  
		Last Modified: Tue, 04 Oct 2022 23:51:03 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:3ade61235c79e10abed841ec509d914a8b7464e9ae14a315fd31bd4e30731572
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51203066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b2cdf463bf66ecb090483f8b819d916678ab23e3fb5f63da0d71a7cba7a0bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:52 GMT
ADD file:887aa5460e148ba204780ebe976e5627d5f4d0a07faf22b86afe146998d75d79 in / 
# Tue, 04 Oct 2022 23:39:53 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:40:00 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:98d78922e3457a6697f2cdbddaab27dbb47e2e0beedb1a4348c56102c850b343`  
		Last Modified: Tue, 04 Oct 2022 23:45:58 GMT  
		Size: 51.2 MB (51202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3485fbd8ba919fcb6b2caabacf6a1da50f715e6983f1dc52019572e61f2211`  
		Last Modified: Tue, 04 Oct 2022 23:46:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
