## `debian:stable-backports`

```console
$ docker pull debian@sha256:225cc1c51acf84f02babc0bc353a2d4178368220533340916da3e00610a0634e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:503715580fea25477efab424d660fb14f5c90695ec4eee9d363f55aa85baffb9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50387707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbf58805393b76368d24d7a2a3418d3019bfbe3ddea13368239982d60bba608`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:23:00 GMT
ADD file:e9c40bd50f470b0a7b37d1ab060af34f57c76aca440f0b1d79aab4e8910ee17e in / 
# Wed, 13 May 2020 21:23:00 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:23:06 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b524cedb63ffa97ab17d2647036a25750d2dfa4771dc136237acbcfb09fa0462`  
		Last Modified: Wed, 13 May 2020 21:29:30 GMT  
		Size: 50.4 MB (50387485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcaf5e6e52801eb9a61f29b168d00c0e8fc6c1cf915b4cddbf49ce29b319aa4`  
		Last Modified: Wed, 13 May 2020 21:29:36 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:fab9edb3dcdc113e77da2609fa4ce20435d3b34ecb1668c7716d5942e00e8a3f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48107705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5031de67ab05ba72843e84b30daf551ed5fc4b1a6c4e49ebb7eac01299eb0ffb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:41:29 GMT
ADD file:d1aef57d1a5b34398c818110de21a1d940af4d8b47d276fd8484e18f91dadb0f in / 
# Thu, 14 May 2020 22:41:32 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:41:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:02a1dacdc62f1fc0c3bd38a053f4d5e023aad5e52973e23a778af71ef38abf38`  
		Last Modified: Thu, 14 May 2020 22:50:05 GMT  
		Size: 48.1 MB (48107481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3eafa9e37268f2a8e5cb8c88c5e8e648e26d0580725097a82f533e3b7da2ff`  
		Last Modified: Thu, 14 May 2020 22:50:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:2aa05adf951bbb816c3bf2a15513d211aca60d99f3506504c00633d6f504e964
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45868787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac255bbd453501e31b9ec6a0854f4658d63821c324530043c907c5339451bd8b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:05:11 GMT
ADD file:18e43632e3bec83fe9bee36c0ac7b8cb186cdacb075fe9b456dc2d87c9240b9e in / 
# Fri, 15 May 2020 01:05:15 GMT
CMD ["bash"]
# Fri, 15 May 2020 01:05:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6da10345cbd55ece785986f0c4a2cdd41a164058eaedd75954a7942902e90608`  
		Last Modified: Fri, 15 May 2020 01:14:08 GMT  
		Size: 45.9 MB (45868562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5904e7ea06e554132b3abadcc41af51a725bdd2f4d847fb63747e4a7df027d`  
		Last Modified: Fri, 15 May 2020 01:14:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e3302e7f49fc7a4f05741b765c142eeedcd2c41ae08f48d8d2db2079f81f3cff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49168431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af55b82d6e639e99f678e7715df9083874a9e54dcc56d13455cdf004092499f2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:46:26 GMT
ADD file:834efa6ef9a13c35ab72dc6a73453ac6cc7033ad45c00eaee6a8419b11ef1a2f in / 
# Wed, 13 May 2020 21:46:28 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:46:37 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d4e97e57656451a538b8a11ffe5155f994ef3442904490aa0382bac955ce5dcf`  
		Last Modified: Wed, 13 May 2020 21:55:26 GMT  
		Size: 49.2 MB (49168207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63814573b27fafac27f727c3f09bbd908a16699a9bc9f2d1daab70b835bdb6e7`  
		Last Modified: Wed, 13 May 2020 21:55:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:b5a3782dda1914d491abf2c7d80610dd7280082a323bbce3dd31b4e7d4fe0f54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51154070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45d4bcc2e40f46f34efd99c84bec41a48dbb1ec0c9a629e398a80b72a11e287e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:49 GMT
ADD file:62f39b7b3178937d8163f0f9d653af6b0a8f30bc47fd77276588c93343009410 in / 
# Wed, 13 May 2020 21:41:49 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:41:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2b8382d3daf21cc75211afcc47e584b30c43e3830bd9b7e8ccb8a44e649385fc`  
		Last Modified: Wed, 13 May 2020 21:49:12 GMT  
		Size: 51.2 MB (51153849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b94829fbcf595608f89f1fc5dce3069bfeb1b4c59075586f7cf88a2c375f3b`  
		Last Modified: Wed, 13 May 2020 21:49:17 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:1a85e4532381375bd8ce67442f82108eaa469b89b0b2e2ac41dcee4e7170ac01
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49019560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c72060cb3d8a0d8fd1b4c188aa520c8bf4bb50693074fb770a4afe58411a3375`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:50:35 GMT
ADD file:297094753c285b8090e93e4efc6845748e298841634aeab712bbf500293c6b6d in / 
# Fri, 15 May 2020 04:50:36 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:50:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7382740eb20031383c40390c748bdb7dcda4dd5646407efb3fdfab8f03ba7a0d`  
		Last Modified: Fri, 15 May 2020 05:00:31 GMT  
		Size: 49.0 MB (49019334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce3c3d29731b50a40c9a71c7f3b21724763e6b86f7c4d36e6366e840d1d15b2`  
		Last Modified: Fri, 15 May 2020 05:00:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:bb6dff55aa3f3189e19680c31e34aec518129f5507c356ebd1940d12d5780d6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54143123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f20b4a9f4442b4e84bcd9ae23cc6bce943c506c66d84312e7d2f0db6c81864`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:32:22 GMT
ADD file:296f641446f4b6d396b6378d99ab61ff3b817c0f258164385036cde43e567805 in / 
# Wed, 13 May 2020 22:32:27 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:32:44 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:716f6a705248af2c22382be4e8cd18e0c5fc7c0057547475e6f010cc29c16221`  
		Last Modified: Wed, 13 May 2020 23:00:57 GMT  
		Size: 54.1 MB (54142899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13865b1e6fdd0258be511fd6a1c3710eb887054b8d34a6e9d25d8c931041b2c6`  
		Last Modified: Wed, 13 May 2020 23:01:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:2ad4afc3caa151256e133325705bd8aa97b9caae2ab965717f550a292edeeb8a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48966676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b12f96467f205556e21bd76637ba523518657526aab87caf23b39f9da6ec4e9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:07:51 GMT
ADD file:19daed53e6a44420cf1d9b476137d0489a22cf2acd1c98ccee509d4507f31878 in / 
# Thu, 14 May 2020 23:07:53 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:08:00 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2eb0ffe78e96cd61cf26575faacc9a51e05d50a4f1601a4feb6f4c9e7adf3bd0`  
		Last Modified: Thu, 14 May 2020 23:12:26 GMT  
		Size: 49.0 MB (48966455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d9b300b6cc58a8f07a1f910227b2e722e54fd1c617cb48121225441f89a72b`  
		Last Modified: Thu, 14 May 2020 23:12:31 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
