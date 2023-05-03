## `debian:stable-backports`

```console
$ docker pull debian@sha256:f2887ed6c64581e9ba474926a1f1c8913dae4b77500e87744008bc9022b828da
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:2d06dd1889e83c523bf94814fb2e07c51f7d2e09937d50751de03ef25a303151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55049295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c122435768d49c87ab83c56afa4d4d91d8d875d93c6a2fc6e00de90d73eb865`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:58 GMT
ADD file:aca9ba794e6ed1062dbb831089b8d9c18bf7bb6c8194581cd3e1fb5e80e527bb in / 
# Tue, 02 May 2023 23:47:59 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:48:01 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6a918b9b11d0639c4549e67523a135bcc5e27da3087ddd02fa97bf8c8e71ec24`  
		Last Modified: Tue, 02 May 2023 23:52:21 GMT  
		Size: 55.0 MB (55049073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94b7325148dace42761b8c59bcda56128837c69bc252354ced5471bb9500888`  
		Last Modified: Tue, 02 May 2023 23:52:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:341fd50108bd3aba0518d71cd1b6e70d9539727cfa48a6293a1741ab509eaa30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52546777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d1def12edd05ed53e354e5bb80dc1f617fd509263e921243835e4db6160988`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 22:49:13 GMT
ADD file:c83b51e96ccad1a3bcb3eb66359344f33591342477906e3c6126dc64c2c5e6cb in / 
# Tue, 02 May 2023 22:49:13 GMT
CMD ["bash"]
# Tue, 02 May 2023 22:49:15 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b8f5ba560106b14d65311aa93a26b6d47c0e2897dbd43f82d54c575c8a32e890`  
		Last Modified: Tue, 02 May 2023 22:52:18 GMT  
		Size: 52.5 MB (52546555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46886077603280e7e7b77f0c493193070666352d589c920196d44a7527ee6b2c`  
		Last Modified: Tue, 02 May 2023 22:52:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:978e5ce0c89046f8bf36018fe438ea67b7ac2c4fc2fc35abddfccf7d4904a1eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50210176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dd4cb25812666d2e4c2a0d8e6a0acb65a358c4c3ef83b6957a60272833262e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:48:58 GMT
ADD file:bd7b78868df2f366668d4abec889c7c47a51bc49c119d06e1532b358705588da in / 
# Tue, 02 May 2023 23:49:00 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:49:03 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:56ea246ed583fd11864d13dc48c323cd3595d336d72ecf3fcb3ac27d728aeb49`  
		Last Modified: Tue, 02 May 2023 23:53:34 GMT  
		Size: 50.2 MB (50209954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221337aebf22c0ed7a01a3f93008c7851b6add5e5c4bc5c3070fb3794c73a706`  
		Last Modified: Tue, 02 May 2023 23:53:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:cae2a3c2c13acc1c0e0b206cd7638b185a938fc8dc118da3a1b5ef5ff6bb3117
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53692946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca856c832831605fa44c329d5ee48747563fe05ca96004afdf5d2075b80a384f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:23:44 GMT
ADD file:1b5b1f6a436fc60c7f10320d03aa7b1b6faaebab3a3322b848972a416d79cd56 in / 
# Wed, 03 May 2023 00:23:45 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:23:47 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ecd90e713f50683f93b397fc3ff782094985d4a6b8c735479681b758a711e0ba`  
		Last Modified: Wed, 03 May 2023 00:27:40 GMT  
		Size: 53.7 MB (53692724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808c3c077db38207ebcb9420aeaa7282764a7e8192e18ace53d990d908ade05f`  
		Last Modified: Wed, 03 May 2023 00:27:47 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:7407d93e39e6773c5278cace38cc9a3cf527a88daeeb246f44b53f2f5d94b91d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56029382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e594c1aef733536579cadb4a7da1b2486cc3533ec550dceb7952f1a1b6960904`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:02:23 GMT
ADD file:881d5b53b693ab267b2b6375d634efd9c5f899b33e26c45a13051a1007068c44 in / 
# Wed, 03 May 2023 00:02:24 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:02:26 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1fba5be5703f943a4656bee5842429a16149e84ae626eac6197cae2a9aca75c8`  
		Last Modified: Wed, 03 May 2023 00:07:29 GMT  
		Size: 56.0 MB (56029162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d178a6e886c12acb44822ab800b6f7cb9888102ca3cf3c1644f7cc8480aa137`  
		Last Modified: Wed, 03 May 2023 00:07:37 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3db0fdf9731ee1fc92317209527f7e82ffb73af833344d8cb6a116351b5645ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53261334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e43540b8cabe8b532a0f6b829d5560a071f0c13876a91945c9a6b33c5066261`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:51:33 GMT
ADD file:43167db8d8bb6eb21b21ec94218332f87cbc663105a0e946ed7d4ec1a8a70d54 in / 
# Tue, 02 May 2023 23:51:39 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:51:48 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:495449cca4f79cc185e4a7402bf7e50c477c6d377274a5967a832e638429edc0`  
		Last Modified: Tue, 02 May 2023 23:59:58 GMT  
		Size: 53.3 MB (53261109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c03ef15705cf712610c6e81e186a6903a712db696e682bb267fafbc299ca67`  
		Last Modified: Wed, 03 May 2023 00:00:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:c833373418faec6398635336a00fa6ae95a6026a7ff7e28e4e99409308e93356
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58924250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca00688698d4574a32a882c99b8637bec49416373bfb2829f4547a89ed19daee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:32:52 GMT
ADD file:11d9cf4961d8256057c0bd6a748f37fda7b0a8e22ff33ca79dc9a781f7205407 in / 
# Wed, 03 May 2023 00:32:55 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:33:02 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:260717649fe5df2b755c3c119a61e9bf051b36456f8dfed0999df48a44615be9`  
		Last Modified: Wed, 03 May 2023 00:38:03 GMT  
		Size: 58.9 MB (58924025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0b5e427e87edc8eac3e7991aff64e1a768fdf3f33518bef4039bb8fbb3e3c9`  
		Last Modified: Wed, 03 May 2023 00:38:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:28906673e3c556c941f22beec0fb48999fbc973af331ab89ded0c699de79c6f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53286862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9ca89831cd75c91f61e181c73bfb1a3274844d01b88fb439dc949892dd6fb26`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:02:12 GMT
ADD file:d908f7342fbc7989444ac877c02229855ecdfb585dcfbaa86226e9e113a75619 in / 
# Wed, 12 Apr 2023 00:02:21 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:02:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:961df1f0f4d8c3e7504abcbd51340fff9c1714f466859ca0077ecbcd6367b5ff`  
		Last Modified: Wed, 12 Apr 2023 00:05:50 GMT  
		Size: 53.3 MB (53286637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9e7a2d5db75aa25aff8e34e39b762190553c497a302af8a391c56c8ac8336`  
		Last Modified: Wed, 12 Apr 2023 00:05:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
