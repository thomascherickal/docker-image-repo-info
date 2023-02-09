## `debian:experimental-20230208`

```console
$ docker pull debian@sha256:ca9b36c8f14356858f9532e0b6fce908327eb7f4ef6988c9efc9052b667ac8bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v5
	-	linux; mips64le
	-	linux; s390x

### `debian:experimental-20230208` - linux; arm variant v5

```console
$ docker pull debian@sha256:9215c9972f2e7b1b1342dd6a2caebee2a65d69a8f5a7eb4f3c6cc1935451f69a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48168889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1ecfe735c526cf2981370208c40b909a893104a622a5256631533c5627ff06b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:02:02 GMT
ADD file:7bfd7547d6a26fb6099d06f79d79da7b24a066fa5653edeb1d00ef2abd960ab6 in / 
# Thu, 09 Feb 2023 02:02:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:02:20 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b06d379532bc5b3ca4ac0683130115e7f1789aec62e79fcfa5d1d3d3c2da1dc1`  
		Last Modified: Thu, 09 Feb 2023 02:08:08 GMT  
		Size: 48.2 MB (48168669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfa7a9197fea7f947656cdc44a2acd386930874401d8e1ad3ebc196ea9967e`  
		Last Modified: Thu, 09 Feb 2023 02:08:36 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230208` - linux; mips64le

```console
$ docker pull debian@sha256:62ba174e8e2f575c50ab2c45d01e7a396d01dd446a103001e3f120e4dfff277c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49094483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa283049093ac699beae3c7c914a1b433fb6800399379f622365d0fff35cf1e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:49:42 GMT
ADD file:d66b7879da96c52ddc9d32b677f67f6f36cd8d58f06b6fce3c4c8720b80418da in / 
# Thu, 09 Feb 2023 02:49:47 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:50:33 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ed54f16bbfa6ae7109ae525fcac7fae8fd6ff2d232ff21349cb18e393290aca2`  
		Last Modified: Thu, 09 Feb 2023 02:58:13 GMT  
		Size: 49.1 MB (49094261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4bf8b3630a4c4950dd6d9854e5179d4d9e2572d1aea943c66b630153abc0f4`  
		Last Modified: Thu, 09 Feb 2023 02:58:51 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230208` - linux; s390x

```console
$ docker pull debian@sha256:8dd2352eb6e9e45194168e322f485918dcf0c9213c94e4b23b5c69cce1ba7fd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47605717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9548917f655bf29614914fdff2fbbf2eb7723b75a68bb30fb8b5a83ceb1168fb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:24 GMT
ADD file:a9c6323e382aa32d6b596f1c61f55f06e55357b5ad0ec8c4027bd649a9183d73 in / 
# Thu, 09 Feb 2023 02:43:26 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:43:44 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4f6aa1d95f253f3246d1d60386fae207367e7878c935165536d9a95adf2070f1`  
		Last Modified: Thu, 09 Feb 2023 02:47:43 GMT  
		Size: 47.6 MB (47605497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0889a005301a1bf2439763c04be432e801c658228a3ad297c33d4a4081b47d`  
		Last Modified: Thu, 09 Feb 2023 02:48:00 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
