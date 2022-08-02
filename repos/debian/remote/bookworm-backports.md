## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:aa250e2fa04018aa691a8eb504d57ad35d740c8f8a8f61416578aa126dd3296d
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:a969a819418bd4bfd10124af67afafe7f2539e74b394bccc69af430df2987721
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53004615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835a5192ab5b8a6077bfeae060e03e406d740f450145ac46e14a488c6a81227d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:34 GMT
ADD file:44585678df56989e743f0dcdebdd7e185769e100eba2a84aa9ae93a96dd39d04 in / 
# Tue, 02 Aug 2022 01:19:35 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:19:38 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9777db7a6b5e969eff343df5e4a008fcdc763cb3605175224b012d40044c2abb`  
		Last Modified: Tue, 02 Aug 2022 01:23:07 GMT  
		Size: 53.0 MB (53004390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfc5fa3e6359cfea2c74ba93a5b56ac3b7cf678b133bd17fc45b70e0261763`  
		Last Modified: Tue, 02 Aug 2022 01:23:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:b5260df8be83b1f532a8a4c382de3a1ba1bf1e396485a52ea57bd2277b85532d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51813162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a26ea3704425eed3a1bb4bd309f3ed7cc28301a815c7b627118948bd375076`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:48:33 GMT
ADD file:f83bd7c88ccdb8f7b53f9072524438c8262a71b297a007c804923fd6d817479b in / 
# Tue, 02 Aug 2022 00:48:33 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:48:39 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f721a266d53173a0af0b138649440b41e425660c1bfb8506b479507fa2627c4d`  
		Last Modified: Tue, 02 Aug 2022 00:54:42 GMT  
		Size: 51.8 MB (51812934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2442bfe55f85538ef0bf436782693f3e88a51a85357b58e63a9db7e49a5b8b`  
		Last Modified: Tue, 02 Aug 2022 00:54:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:76355ceab3c45b90951997c1bb9482f0bc6edb4e7f67714a35514252908372bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49527902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f061ddfd3cfded93d8c9eacdabf6e96d83b5e9011d9261fae62c2786b676d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:57:55 GMT
ADD file:359193f5179bfdc5181bda2e05bd0b22ae4a86c638b0bbf09f289d1727fad222 in / 
# Tue, 02 Aug 2022 00:57:55 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:58:02 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:537407bee93780ba0135c6d74e62d8cee8d32e85ab926669d3cc9bedeef28852`  
		Last Modified: Tue, 02 Aug 2022 01:05:20 GMT  
		Size: 49.5 MB (49527674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5170da6bdf71d91cfde82888c8b63fe15f40c19cf4cf3d2fab4a14663bf1ee4c`  
		Last Modified: Tue, 02 Aug 2022 01:05:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7b49315cbbf368c7c7afb6fa3164c3a8fb54389068d30f2b88cd387b4b3bc8ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53097717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0eedd6372e9185ecfdc1dc69d5f97394321333117949aea299cc96ed038895a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:01 GMT
ADD file:66ffd29b395276f108023b4be1a449714b6fb1fcbcaf770debb7ec6910e84294 in / 
# Tue, 02 Aug 2022 00:40:02 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:40:08 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c76fc726ec0ec853818bf6b42fbe47810086904b89f146d4ccce624e8c5a33e2`  
		Last Modified: Tue, 02 Aug 2022 00:44:53 GMT  
		Size: 53.1 MB (53097492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70597b8e0d494b5d4f995fb718428c69d3fc7229827324279e78ea60b3bfe29b`  
		Last Modified: Tue, 02 Aug 2022 00:45:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:6e28f291a2a13c486e3ba337fa65bd39c67b4abbe441cbefa879ea051e221049
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (53974293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b05b7fb112635993ecd2f93b974f5b79e7e612ccd59d3ffea8e35dd08cf5b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:38:40 GMT
ADD file:f331e5b0e8626bfcbb682d701943586f63db1ff65d9add0d94759ecaeb8c8269 in / 
# Tue, 02 Aug 2022 00:38:41 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:38:46 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f78c3dc38f418186e278713175ef4cfc4bc70d85867d3597da89d03b5b956170`  
		Last Modified: Tue, 02 Aug 2022 00:43:55 GMT  
		Size: 54.0 MB (53974067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a0b76a11026fc6f9f0c7db34faa1822549327a235bd3d880f3a6f6d5ed6589`  
		Last Modified: Tue, 02 Aug 2022 00:44:07 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3f8d4c87806092ec9c08251f31a50eaa174b069ccd65d141a8b02715b6be0336
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53100086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a6469fb1c4843e69e4d009d98b2c39fbb9eb90ba1cbd528d5b6d257dce3829`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:08:47 GMT
ADD file:071fbdfd189eb16d9f6ef75de927dc676c1f54b47bc4e17163522108782b28ec in / 
# Tue, 02 Aug 2022 01:08:52 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:09:05 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d875d0bc6e0221f25e9536bae93056c28a4346ebdefd9847e38ca0c0b536a4b7`  
		Last Modified: Tue, 02 Aug 2022 01:19:01 GMT  
		Size: 53.1 MB (53099858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d51cdc98b5b5f63d47c78b37be4f1a31392fc1aade3d9b9189c4a899912611f`  
		Last Modified: Tue, 02 Aug 2022 01:19:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:589e3d9382da7e2a415b14f90f20b1b2ebb4367af1ccf3ec873d6decc27bf967
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57222005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647f21aa35892af53c6d163ef8e383ca911e0cab4611c9e543419c6ca672c592`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:16:36 GMT
ADD file:c74b95bf7c5e132f531cfa82f2087d3674d54ec0a5ffe1b63c3b2c23982544d0 in / 
# Tue, 02 Aug 2022 01:16:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:16:45 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7626a07e3e0f205ede86e25585175b90c4c7ab30a82060614ed072b13dcb055f`  
		Last Modified: Tue, 02 Aug 2022 01:23:07 GMT  
		Size: 57.2 MB (57221780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f491399bcad4cfdc6bb3569b43d2dfd1ca940a975fa59d7cfb6eb34833ff52`  
		Last Modified: Tue, 02 Aug 2022 01:23:18 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:b9b7d05433d4e6b44f87edc9c659d5f28f4ebcd908c84ad95b3f9d2f2a6fa732
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51514758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4a485160e441e4846244d010a33461bad29d824c6779112a1d5a67482146288`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:9364324d9e3e24a6e417365a226c42bac5c3c9589b444096a65d5bf539eec127 in / 
# Tue, 02 Aug 2022 00:41:45 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:41:51 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1a5bd7c6618b65a5948f8c07805e4109ef4f5aac36711b43d0fabe6f11fe0ec8`  
		Last Modified: Tue, 02 Aug 2022 00:47:13 GMT  
		Size: 51.5 MB (51514530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee872c14e3a645e96ac2b8309120462ce84255706cd64d1d2d1a153b5310aa5`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
