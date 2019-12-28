## `debian:experimental`

```console
$ docker pull debian@sha256:56799b53515d4b2d10b95d0f67a70338d83311047da3d01224e9000201d0f46c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:eba57eacbca97c17270138d5cddd6f59d21397d37a95a168385306a09e0e8588
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51479802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dbd4d69c683df8ec97d5641adb419665476d914d158322d5ebb60c741d18e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:24:25 GMT
ADD file:35e647c520930c73f7b2e881ca8bdc41af44b37c0609a6cc814849c5c705cb04 in / 
# Sat, 28 Dec 2019 04:24:25 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:24:39 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6d56bcabd317031388b00edfaa5836907d3c755109f521d1a049234760362418`  
		Last Modified: Sat, 28 Dec 2019 04:29:17 GMT  
		Size: 51.5 MB (51479580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f4284c7f12a870f035bb9213a3922b3322332409fbee4220f8f976ccdc5f74`  
		Last Modified: Sat, 28 Dec 2019 04:29:36 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:87ef2d3c7fcb155b57a6323c88f7cfd01453244134964dac951de309df84ac64
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49263353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0ea23312c134b0d25d2a6636c525ed5032a7c9cddca449799164f9b10db7221`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 12:19:37 GMT
ADD file:9d2230ee3ddb138acdfee1dbd29546c49e9e32ee34a74a60ebdf7b6cfe3cae57 in / 
# Fri, 22 Nov 2019 12:19:39 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:20:09 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b6ea9592ed328b6eb0b0c4a3141002e269634ec35f8143011d74b53cda3ae314`  
		Last Modified: Fri, 22 Nov 2019 12:27:24 GMT  
		Size: 49.3 MB (49263130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9be66189ec6ed7a31560b2239c9199afce748dc7b473a0b4cd945347806f1b`  
		Last Modified: Fri, 22 Nov 2019 12:27:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:1c4b3ebda32910e68e07e9dbad4d732f780cc5e11ca1e9c4350705f21532cd07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47016145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b360a9d213a6ea5363fc41173e72eb60571ac1de8a9ba0863d7eb90bc2c1b5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:30:48 GMT
ADD file:1ab70b89f948376401410c757c49f8781992ac450988f9033925f9e30cdf93dd in / 
# Fri, 22 Nov 2019 13:30:50 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 13:31:23 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7bdecb16b8751d594825e3508d93c9c87c76ab4d164063ab2539a98223f6b99f`  
		Last Modified: Fri, 22 Nov 2019 13:37:56 GMT  
		Size: 47.0 MB (47015922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8136af8071daef364108609350a3326f3c1f96d03b76c43f34efd508c4df0d1c`  
		Last Modified: Fri, 22 Nov 2019 13:38:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:5fb8ce53bfd68fb9b60eaa63d3b027b139e9dbffc5ce71fc22a556092b46b0ce
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50259415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6cac0c24350549a906a848ca1e893409765ccec0da1264f896318a6ba68abc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:47:11 GMT
ADD file:7920e829dfa046db84f6b7dcb836b681da9b21dff6a09b3917615a40a280d880 in / 
# Fri, 22 Nov 2019 13:47:13 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 13:47:48 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4ef86084902b058d766d1d667217f9936fb3d72a21c2d420cecd939a8bfc0ff9`  
		Last Modified: Fri, 22 Nov 2019 13:53:17 GMT  
		Size: 50.3 MB (50259191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0582c5d0558c594b31e04c028fdcd9cd860dbd345060647808818831b8479ca7`  
		Last Modified: Fri, 22 Nov 2019 13:53:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:40139389d502361c56241dd2cd84690eec5aabe598052c3a60ecacd26149a6d7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52411593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f48a9049907f5d9b5a462a01e2492ba0b0491153fd08834e71ca993a63f8e8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:56:07 GMT
ADD file:93ef34233ccf854a8bf33b4d9336a1fad64d2e2925a57c74559f165e91767b40 in / 
# Fri, 22 Nov 2019 16:56:07 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 16:56:35 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a1caf6679d73645f9740ae75d7098da232e5431faf957233db1d2084d88c213a`  
		Last Modified: Fri, 22 Nov 2019 17:04:05 GMT  
		Size: 52.4 MB (52411371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb278dce04d784553175f06166d34ad35b3e3c8ddb295bd1f54200b4de8ca7d8`  
		Last Modified: Fri, 22 Nov 2019 17:04:25 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:d8db39195028ea481eb4ba947e98b226af3be0d692c2c62e895b6c951197e840
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55285258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8224672254e14ed5eb873403cd5f427b2f00829bb02c2a4ba32ae2dcb1c6ea2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:24:23 GMT
ADD file:3fa43243b74fbe99581623505a389cc44baeb4e9ae39ba949e4e1fc50450e3c0 in / 
# Sat, 28 Dec 2019 04:24:26 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:24:48 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b37639cfed2fda912429972fa7eb754c58acaec8182ef1c9a65f22009dd2d37a`  
		Last Modified: Sat, 28 Dec 2019 04:35:21 GMT  
		Size: 55.3 MB (55285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa907c7433a0fd42c41204b25108fc32aca62fdec03232081f84fbb514c0acb0`  
		Last Modified: Sat, 28 Dec 2019 04:36:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:65a77c8c75fa7d7e77f17369cc677d1ed118905e22480262b5c9caf8d8296703
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50131791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6e531289ae014aae792675ccc8f1cdbdf706c79b77428bd4069f134e991d33e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:51 GMT
ADD file:92150dd1aba65cd0aabe0f7308e76f8cf6118359acfc1ce39390212c2c196752 in / 
# Sat, 28 Dec 2019 04:43:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:44:03 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:58852c647a6833ec26f1478a3018cda4b626ae58859ef852ca6f88bd639a45b6`  
		Last Modified: Sat, 28 Dec 2019 04:47:14 GMT  
		Size: 50.1 MB (50131570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f35e79442cbc0cbea8a9d0e5d8e860fc611158ca2b9a4a4165b3c162cdb2ed`  
		Last Modified: Sat, 28 Dec 2019 04:47:29 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
