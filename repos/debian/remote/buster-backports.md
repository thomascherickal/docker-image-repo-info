## `debian:buster-backports`

```console
$ docker pull debian@sha256:f0d1476b2a350b4b09cc0e934fabe8a839a354633ace949a2654a226b62811ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:77ba988d4f876abf86c615c4c8ac0a7705ada95e4615c89580f30087e06470fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50447964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d4d659a63a1d67038f74772d83a8bffd8e5fb22b1462f1d1aab02fc797cd06`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:02 GMT
ADD file:259be79d94a2549a667ad08a093fe18f15a6c93d66a0723292f49294e31fc7a1 in / 
# Tue, 25 Oct 2022 01:44:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:44:06 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fd31ec14dccdcda8f2472547f1a94ef0a23b8dabb764cd7b1d48aeee0afea7c8`  
		Last Modified: Tue, 25 Oct 2022 01:48:15 GMT  
		Size: 50.4 MB (50447742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2814ff3db73b71da97af63bd15cc964e7cd761db5fea54ff563e5e24d65f9`  
		Last Modified: Tue, 25 Oct 2022 01:48:29 GMT  
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
