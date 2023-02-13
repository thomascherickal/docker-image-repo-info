<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `clearlinux`

-	[`clearlinux:base`](#clearlinuxbase)
-	[`clearlinux:latest`](#clearlinuxlatest)

## `clearlinux:base`

```console
$ docker pull clearlinux@sha256:9bc381749ce77850f39095ccc2575f88752123df0e50588f30211f9c82dcdc49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:base` - linux; amd64

```console
$ docker pull clearlinux@sha256:9b8af441e1eedb51c8e038935d0d7e4b75709a0758635769c00a715b743cd5a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86740654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b84ca664f406b0c37d86b226359c3b8f5049ab75bb813e14c21a8dcf936bd5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 13 Feb 2023 20:24:12 GMT
ADD file:153449e3cd4441e7e432c5c5a05dd620de69abcaad20bccc03438ea13730caf1 in / 
# Mon, 13 Feb 2023 20:24:13 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 13 Feb 2023 20:24:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ebe187cab3716203d43dbe9f0e3a4120df26b44835685a31ea528bc76621b2ac`  
		Last Modified: Mon, 13 Feb 2023 20:24:34 GMT  
		Size: 86.7 MB (86740436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1a530e8cf85f3667d2919ec39e5aaad839a0310c42cd87c945d0ebc44a8f37`  
		Last Modified: Mon, 13 Feb 2023 20:24:23 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `clearlinux:latest`

```console
$ docker pull clearlinux@sha256:9bc381749ce77850f39095ccc2575f88752123df0e50588f30211f9c82dcdc49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clearlinux:latest` - linux; amd64

```console
$ docker pull clearlinux@sha256:9b8af441e1eedb51c8e038935d0d7e4b75709a0758635769c00a715b743cd5a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86740654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b84ca664f406b0c37d86b226359c3b8f5049ab75bb813e14c21a8dcf936bd5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 09 Mar 2021 00:22:54 GMT
MAINTAINER William Douglas <william.douglas@intel.com>
# Mon, 13 Feb 2023 20:24:12 GMT
ADD file:153449e3cd4441e7e432c5c5a05dd620de69abcaad20bccc03438ea13730caf1 in / 
# Mon, 13 Feb 2023 20:24:13 GMT
RUN cd /etc &&     grep root /usr/share/defaults/etc/passwd > /etc/passwd &&     grep root /usr/share/defaults/etc/group > /etc/group &&     grep root /usr/share/defaults/etc/shadow > /etc/shadow
# Mon, 13 Feb 2023 20:24:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ebe187cab3716203d43dbe9f0e3a4120df26b44835685a31ea528bc76621b2ac`  
		Last Modified: Mon, 13 Feb 2023 20:24:34 GMT  
		Size: 86.7 MB (86740436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1a530e8cf85f3667d2919ec39e5aaad839a0310c42cd87c945d0ebc44a8f37`  
		Last Modified: Mon, 13 Feb 2023 20:24:23 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
