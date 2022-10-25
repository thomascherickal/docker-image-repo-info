## `debian:experimental`

```console
$ docker pull debian@sha256:ddc1c9a4be660e92d2eb8736e535ebb08ad3b6ecbf22082018f2e0e8e76ac897
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:154fc729cc812cedeeca8446d15d9e344067e351aacf4856156c218bf0e835a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50641427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:061216c4987060efde1cba818de03f256d65af769f5e0c726c47e3cee89519d9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:45:38 GMT
ADD file:1547e086dc40d3418e8f146e3b7fe2141ad7659675f0a810d3723f618ce685f3 in / 
# Tue, 25 Oct 2022 01:45:39 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:45:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:37185fef75d9c859c0943d1efbb25a8ccb6052762fdece7628188b1dd148c6b2`  
		Last Modified: Tue, 25 Oct 2022 01:51:27 GMT  
		Size: 50.6 MB (50641207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187a9a9e5cbb08d19f59ebb1026adfa6311b7d5962ee3eb8789bf89adea76029`  
		Last Modified: Tue, 25 Oct 2022 01:51:49 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:123e4bded6d9d373f7b00f113a47649e15136e6da333cfbf25489c481fc22fe8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51569191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2976aa5780995072a984af827c93291ef5d5aada6e806984578641ccaaad05f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:50:33 GMT
ADD file:bab1d7cd4f6fff2227b43a60a1fb7c76956bf7bb688930cc604b467f461d86f3 in / 
# Tue, 04 Oct 2022 23:50:33 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:50:47 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7237053adb388e0dfe2cbaafd0dcccd406d1b10c7030c164ed81852630a64ad6`  
		Last Modified: Tue, 04 Oct 2022 23:56:24 GMT  
		Size: 51.6 MB (51568970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c533a220a405351670d82020558a83dc88ab84bec30b910a8aa5a729656549`  
		Last Modified: Tue, 04 Oct 2022 23:56:51 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:d02b8d3583936f1d7a6f9b1a448bcdfbe56ab7a3230aeaa3a1b14006dc35964e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49437044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0d6f6d6edbf23da96bfa204aeb64f76a5533f5961ba18972a42f9962ba8db0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:01:25 GMT
ADD file:92caf1a4811a0dd5bf66006102d1354e6d3292692896e2f516e4907290dd2c50 in / 
# Wed, 05 Oct 2022 00:01:25 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:01:42 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8056476b44f05fb09db3c971c46cdd798ed983a347d2ad04b59452136708e928`  
		Last Modified: Wed, 05 Oct 2022 00:09:07 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a7773e39f91c6d4a2c72292e82f5093cc4d3f2ee00b77004433ca4dfa18e06`  
		Last Modified: Wed, 05 Oct 2022 00:09:33 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b10e1743cef0ebd082d94f2a170ede7bb904da7863fe6626d89b28157bbef324
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52700212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c589062a6fb00ab07e5a97777d479d85ceb85f2ca05658727be9b4e9f35e613b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:47:00 GMT
ADD file:648747f4f152d5475b91db660f39083bee7a08b6556e3f2a5b75617fd9bc4614 in / 
# Tue, 04 Oct 2022 23:47:01 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:47:17 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3703d828bb0519d47d75a6f11cd98cbe96f1f12dad3960f016161fdecf0a1425`  
		Last Modified: Tue, 04 Oct 2022 23:54:10 GMT  
		Size: 52.7 MB (52699992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf11604dc48e052d8e37eb1cc1dfe25e82ca0599fa2d1cde4caa1641ef6c54c`  
		Last Modified: Tue, 04 Oct 2022 23:54:36 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:997bce6a5feee727c90a08bf3357448c30d39c51207b64bd1d8605bf76bbc6ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53647689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88c61391c4b6c20dbe12bb681b472a5ecc15bbf495dea2dcad00cf9df37e1363`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:03 GMT
ADD file:c170dc3cf642e70c45596e473b66fc61aa62de10ab2dc638e825dfaf1e046138 in / 
# Tue, 04 Oct 2022 23:42:04 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:42:20 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:546f554d6b6eefde67134c14e4a549c12d1efcd271db7506027d96d7844cff82`  
		Last Modified: Tue, 04 Oct 2022 23:49:22 GMT  
		Size: 53.6 MB (53647465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f21e612b723e4fb8b7a0e474dbcd0842e51fbb277ae92f5439f49e89844e5`  
		Last Modified: Tue, 04 Oct 2022 23:49:48 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:1055ee96fb4aa40bfb557705ff53f831bcfb25d2907570c3d95610b0c841f7b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52670214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a02c4ecaf7b61d170a5a174872007057379522634797acba9c41cf245d026e7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:30 GMT
ADD file:f58a52903d9fd354b39418705999d807d445923c0d906e435069da0c1dcadb52 in / 
# Wed, 05 Oct 2022 00:14:35 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:15:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:568a1dbbc77ecb3e3f3c1bf7be75c0c5280b3cdd49fab44535b884d882f46658`  
		Last Modified: Wed, 05 Oct 2022 00:23:09 GMT  
		Size: 52.7 MB (52669989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36626a52a725d49f5c27919c9cba031479c302e31f98d7ee8a58bb1eec3e1f11`  
		Last Modified: Wed, 05 Oct 2022 00:23:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:0aa855b5cbb507e562ec68992974b463cfcb44dbe7d50d372de652e14bfc04b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56786988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a18503d9127f8199b8e9bbaa29bf946129d4dcc8a3d479fe7d87800210783852`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:20:24 GMT
ADD file:e433f08aeb1a5055a1f595bb9d5d0fa07f18425cbcbe8366d03d37c3220c68a6 in / 
# Tue, 04 Oct 2022 23:20:27 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:20:51 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:272176a2be5bf5f298ca816c92e465b8943131069116a86668dcd55a3431cb10`  
		Last Modified: Tue, 04 Oct 2022 23:27:22 GMT  
		Size: 56.8 MB (56786765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae283b76325ad250614a85d4ec08ef93bdf9edad4b7bcab3f475ac0cd7a8cb7d`  
		Last Modified: Tue, 04 Oct 2022 23:27:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:b082869078579995aa16eeb74f8ac655b4a51d91b4eb9e7aad33cb7752b3d2a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48857998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ae6beb27df1abcddfbe6a029718dc63ec2a09e72e74f7aa6e23438ae91bdbd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:43:33 GMT
ADD file:c69bdba9cce2cc03f2cfd44cc313597fa4405db3fb0eccb433d88722ab31e34f in / 
# Wed, 05 Oct 2022 00:43:35 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:15 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ceea310cdd06f4830c3118154bafc9f92a2a516a584c58091678a3121e2aeb79`  
		Last Modified: Wed, 05 Oct 2022 01:02:00 GMT  
		Size: 48.9 MB (48857770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe922ddecfa6a280e6520a82797a6ea2b614196d9919da35bf2b800c0a7510a1`  
		Last Modified: Wed, 05 Oct 2022 01:05:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:3696bfecd4373574428052be1c6bc57f86857903acb5c6b86fb7b0ae9031fb86
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49013157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b736aeeda8a8eee6fc99797030aedd3efd0c0f0c53950bbb63d4993259e6f5bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:16:15 GMT
ADD file:0258dcf1ca7bf72abeb6bb2a139a712f118544a38e38c277acaae984d4312e12 in / 
# Tue, 25 Oct 2022 01:16:17 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:16:34 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ad8b0151e3d93e0406fa9194bfc8fabf5a340300bed913637542073f2f8b0eb8`  
		Last Modified: Tue, 25 Oct 2022 01:20:42 GMT  
		Size: 49.0 MB (49012938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bb1bf872871a010d0b98d4063c2111eaedaa5837abc609668142bdd837da14`  
		Last Modified: Tue, 25 Oct 2022 01:21:00 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
