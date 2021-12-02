## `debian:rc-buggy`

```console
$ docker pull debian@sha256:c115949d99e1e3ab3d9e0e2172264e159a9d31ab155ba7c7a09156779f2f0f32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:58aef7c2ba6b9adbb66c2759591d8fdb77feb356648f582cfe190209465693aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55747092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47eb6d7081d7a7e90539701f7995184c2506e0a03ea54cb8fd8d51176fa3f057`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:37 GMT
ADD file:aa0a8871e20fb4e68758bdebe7ee1e99e982c5e9d2e97b73575b8dcc2ab4adf8 in / 
# Thu, 02 Dec 2021 02:49:37 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:51:20 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:af46a953975205f2d7320842b5338767ad3d4aa084267279fc21cdc807374c52`  
		Last Modified: Thu, 02 Dec 2021 02:56:05 GMT  
		Size: 55.7 MB (55746868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d57dc66ad01e2430ebf314bf8333a5a5ada63c8ee98dfe2734df95cd14df19`  
		Last Modified: Thu, 02 Dec 2021 02:59:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:8a9a5b38b0da9a46dbd20824882dabdb4853d0cd6e1e7f2615a18a3b29b8b031
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53226483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70bd8bc8ded7cd187de2132c45c270bf1c9d8fabb0035ded84933b7e5e42dfb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:54:44 GMT
ADD file:358278336204ee1e51bf00f8c88d281c73e7e5d5b537fca1ddea89c9e69da90e in / 
# Thu, 02 Dec 2021 02:54:45 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:01:15 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:92d580f40fe8bf02becf360f6a4dc76454bfd66964c4acc0ddcd113fa0e9c2d1`  
		Last Modified: Thu, 02 Dec 2021 03:13:27 GMT  
		Size: 53.2 MB (53226256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e4f483f68e28db537a123a3cd732a5e0cee9d639cbf0a264c706047e85ad91`  
		Last Modified: Thu, 02 Dec 2021 03:18:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:b3c4fff805c799adaeb6f303688b2a506eebaeb4fa44b5acd62894106a1d5a64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50860534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd03e682005cb71cf59753fd8cbe2ef48938f59f40dc27f2f581c04b0e63359d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:03:10 GMT
ADD file:df29fec66c741f67158d8ed2094810758d4a7cfb2c7cba3dbe60e5bc11ed824a in / 
# Wed, 17 Nov 2021 02:03:11 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:07:48 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:339de498e0e3324e5657ae3bd0868b26e4518664b7405a1fb321434233c56211`  
		Last Modified: Wed, 17 Nov 2021 02:19:45 GMT  
		Size: 50.9 MB (50860308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3ece82fed24d30367e02d7e64c964b10ccfd15ac07fc7194004f021e5f5a72`  
		Last Modified: Wed, 17 Nov 2021 02:25:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4e643b87023ec376c041e087d96526b897466ff815c93e009c21822054991b27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54767270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef88aa400312f886965b74ff4049517b7b6ae074468393de39d842d82e0614c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:46 GMT
ADD file:6547698ce9c0dce5d390e739342bd015a0c3266dba4ef5828dc1b1a9eb46e826 in / 
# Wed, 17 Nov 2021 02:41:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:43:49 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:67eeb578521bba47ceed6d5c2de23409a33ec3c1c6fda03d83e22d74dc1cdb76`  
		Last Modified: Wed, 17 Nov 2021 02:49:53 GMT  
		Size: 54.8 MB (54767045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481e7fcc41eba4bf5eaf90b91e396fbbd7e3419e82dd8276f76e396ea7836e08`  
		Last Modified: Wed, 17 Nov 2021 02:53:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:a6e3840ee34c8aba615d40b78ef2b33dd56c0924b98402834bbbd12e48f8a7ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56808283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d6cd31f0702be048d28baba1029289a125b2cd30771e6d8ab7bfdc506b3d32`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:41:35 GMT
ADD file:166234c060754022c10737b949088caccb46aa6315aa91f9ff63dd1f60704729 in / 
# Thu, 02 Dec 2021 02:41:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:43:49 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:158718d3425b2eb9ceb4c5321a7633c30d7b948b7dfe2a98608b354788b1c2ab`  
		Last Modified: Thu, 02 Dec 2021 02:51:07 GMT  
		Size: 56.8 MB (56808054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb92de190f82b8ff26faa24395cf567d4f81895aedc0b29654c23b0d1e6c0d9`  
		Last Modified: Thu, 02 Dec 2021 02:55:06 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:ee17048238bacfc70387bf3d6f0c3ad0dac7de84242dfc39c31e64e3ac8e6601
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54455669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:854a08dc7561319bf987b0c21ceb22c22c67c6c6842d581b7b9199f1c6e91766`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:11:25 GMT
ADD file:756c847932d446a78e78b1785e3773acc2f468bed861faa53b3a777f03b1273d in / 
# Thu, 02 Dec 2021 03:11:26 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:14:34 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:851a637e7cfa078b1e4bcb2543d21b6bd9e139295986a256dac39682452e1a34`  
		Last Modified: Thu, 02 Dec 2021 03:48:41 GMT  
		Size: 54.5 MB (54455441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f646d2887aee687df77601b7d6d69915a99c02cb346ee7f9df5aeae696d97e11`  
		Last Modified: Thu, 02 Dec 2021 03:53:26 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:e6a53aa9bfaddca7e79497c6eb40aa1daeea834f9ca4aa6f5cf1c535f7bc9d48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60045243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d425b6bd2dea0e52c16acf25b9f9f40af58d410764f85ecac935b45c8bfab592`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:32:54 GMT
ADD file:33bc17dd3e3b6cd8c5ac37c8382a5d2b8e3ee8384b598b69b0d17b813dcfc767 in / 
# Wed, 17 Nov 2021 03:33:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:41:21 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:60fa303f933c621481dd7a32f72de0e35b85a3567ff116516725c45089e1cb88`  
		Last Modified: Wed, 17 Nov 2021 04:05:01 GMT  
		Size: 60.0 MB (60045015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e724ddafa6e9bd2207878f8f4c849035ecf2ae94dc3ed419e09391e7db9a43`  
		Last Modified: Wed, 17 Nov 2021 04:19:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:6054ea59b35ef1d4279cd624e8d9681ef963b816a6e50612ea5119670b470c59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (53965892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca2d58825e5f75bcee91ad98bff0a56adad0030bf68f202a8b4ef3b1deda14a9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:42 GMT
ADD file:ba3a56dbd46c1324142a33ad1eefa66c34fda8c9c635140debf01131cb259e63 in / 
# Wed, 17 Nov 2021 02:43:45 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:39 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3595b50e30d7d0d412c142596638dbf5abfc27f196fe5d138ded04b66fd2b50e`  
		Last Modified: Wed, 17 Nov 2021 02:49:48 GMT  
		Size: 54.0 MB (53965664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cddf6db144344852ad11c114803127e5c012f50bcfe344b2c9492160f02fb11`  
		Last Modified: Wed, 17 Nov 2021 02:51:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
