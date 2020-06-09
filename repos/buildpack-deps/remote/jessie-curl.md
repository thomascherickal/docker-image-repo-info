## `buildpack-deps:jessie-curl`

```console
$ docker pull buildpack-deps@sha256:17553feb69ce504df7e3d11fd675aea5b18219c21cec09d7ed486dc6ac499dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ab8e317ca15fa25f7291b407c53ff31df73481e9ba3f4b8212007840f5bfbe77
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71933761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f015a0eaaa22aab930ce936e230ead271142c4c01b807fb3f453aa87ec42c5c0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:09 GMT
ADD file:0419e8fcec7ce7e70dc1f1e19558f15ebcd61d43a3b9955811783ac3a56c79ac in / 
# Tue, 09 Jun 2020 01:21:10 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:49:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0cd7281e66ed488ba431fd1e41a3c5fd628ed921f059ddbba2597487962ab380`  
		Last Modified: Tue, 09 Jun 2020 01:26:04 GMT  
		Size: 54.4 MB (54388052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041e5427efd77699a148fcef4a48824bba787ed6c2db375aa3f3d8b97ac92ad6`  
		Last Modified: Tue, 09 Jun 2020 02:00:55 GMT  
		Size: 17.5 MB (17545709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:193f8e469d0de2a3f9d918857dc94bb5d915504b769b1b219d28357ed6c6dcd0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69618807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:445c0128dd5750d58b7e2d9f301b30bfe5320b2b3ea85b54385dbdcdb6456f70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:52:16 GMT
ADD file:4714dbb428f38b9b79a0b0234718dfa1c624973506e8a75c52a1753f4202bf13 in / 
# Tue, 09 Jun 2020 00:52:19 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:33:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:33:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d40938239771bc3bd6ddf7de365dee7a73a438f26b51bd64c09fa994cda5c2a4`  
		Last Modified: Tue, 09 Jun 2020 00:59:47 GMT  
		Size: 52.6 MB (52581526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5029f3fc63be5c726f83ec3d4ab5012e35c3267c5eaa1e83f1614de2fa36622b`  
		Last Modified: Tue, 09 Jun 2020 01:59:39 GMT  
		Size: 17.0 MB (17037281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9c1bcf315305296531003fc27a020786eb315ffb850be27178597fbb4d6b013f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67027874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f3842304566005b04f3e797f4b5c0333c7faa71eb7d160f5e7a0eebcb0ea9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:53 GMT
ADD file:e29fa406906c6574ad0eb78b933031cfcc111886562a056ec9634129c964dc87 in / 
# Tue, 09 Jun 2020 01:01:57 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:53:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:53:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:909e57799b0753688e459363ca5a8b3b97160ae637423d0533fd72503e5ef9a3`  
		Last Modified: Tue, 09 Jun 2020 01:10:48 GMT  
		Size: 50.3 MB (50304486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be3c793af972342b8657d56ce6f318a17f6707d23555d7407bde9347f0349ea`  
		Last Modified: Tue, 09 Jun 2020 02:12:44 GMT  
		Size: 16.7 MB (16723388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:106b02adde9fb102734c9a6e88ba1efdb5b733ee62d01035d38053c2c6fbb4cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74463681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cb824bc9d345cc95a3edf6f4711ee849786a23b3bbcf1cafa6d0c54294316b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:40:03 GMT
ADD file:e6be478576ebd8d188f0f0507591d45863e225be60ae0e6381a7c54446efe116 in / 
# Tue, 09 Jun 2020 01:40:03 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:15:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f753419b4b3c0070d8de5c715f2097d69b60f7b505cc1c31085c9871d67952d5`  
		Last Modified: Tue, 09 Jun 2020 01:45:23 GMT  
		Size: 54.6 MB (54607842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c6dd78519f2dfee7b28710545708cb946bbad983c2e4327254a388e0e2b024`  
		Last Modified: Tue, 09 Jun 2020 02:33:35 GMT  
		Size: 19.9 MB (19855839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
