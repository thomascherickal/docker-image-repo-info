## `debian:stable-backports`

```console
$ docker pull debian@sha256:3dc11e6def94c82c0e6a702e6547eab6fb2990c6d13024b8ac29fe2530a9fca0
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
$ docker pull debian@sha256:be66163a49ace1f23b224d1d4451a228ccd67664a918b614e8824bec7e773482
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55029958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbed3c5188441a08ba51d0dc00a67d86bdfb3b4e19afa67234145e5dab4fc452`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:33 GMT
ADD file:57088f13d9b85537ab9ccd327018b098c2e57f2ee2e1356e79cefc0f2fdc2760 in / 
# Tue, 13 Sep 2022 00:57:34 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:57:37 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f1e379b15ae030f3314a89ab08091556b6908686b2c832074e178f3c24666e60`  
		Last Modified: Tue, 13 Sep 2022 01:02:41 GMT  
		Size: 55.0 MB (55029736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bcfd9c12dcbdba6e02a533812444e4825c6b433bca157e1f5f4a19d9a8bfb2`  
		Last Modified: Tue, 13 Sep 2022 01:02:51 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:0ce7d54f7461a0e16df1ead933956aca3902985f0ceb7cab86dfa28ff01b5de2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52532430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:675beccbc352e917e7e1c45b52bed92fae8eed43fd2115891ddaf7cd51322efa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:54:36 GMT
ADD file:b64be57dd449eb3bd2e5319d0d46632d2c277352b68db8d4a9c45c96896b2de6 in / 
# Tue, 13 Sep 2022 00:54:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:54:45 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:43faf6de0705a21d8ef228cbcb7960b4e2a3bab50c1e4556ea52fc3f2cf9c214`  
		Last Modified: Tue, 13 Sep 2022 01:02:33 GMT  
		Size: 52.5 MB (52532206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836999b221109912811a01ed70ee8bb77cb0a0eb1f85bd4235521f0edcd22033`  
		Last Modified: Tue, 13 Sep 2022 01:02:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:f39724a7b04ce1e11dd52676e10209fd12be2b51d205e8c56868d3ffbd6ea87b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50205158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a6ef7117b84917e2dbdc37f3e6287cd55164c04f7413889720ccb6af3e3dcc5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:45:01 GMT
ADD file:8258337dfc0645ce426d6dd6af19232978c467688d3ce0eb4e074cfcb6814b7d in / 
# Tue, 23 Aug 2022 01:45:02 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:45:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a199ba1ecb719e70e77944caf4b212401d467cfa213206824647570f8212a0fe`  
		Last Modified: Tue, 23 Aug 2022 01:52:45 GMT  
		Size: 50.2 MB (50204936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207e552841c66bbb04456beb89a442fa55fe7be88f41519228c6adfbc82e6f4`  
		Last Modified: Tue, 23 Aug 2022 01:52:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b43cfc61594a77219dd1ae85065d250158cf4c5e1228f04820528ddf8bf2f080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53691077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b6e083357bba07df7dbc64d2720a0846a0dd549be367b480fa4a503185c817`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:52 GMT
ADD file:a2d566809c5b419e9db89df55459a7395fef51ca1219fc7208c6f85ec1563fb4 in / 
# Tue, 23 Aug 2022 01:53:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:53:59 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8de130993eadd6b4f6351b9cb731d73c9d4ef04db732eb615c12093f56a958ee`  
		Last Modified: Tue, 23 Aug 2022 02:00:24 GMT  
		Size: 53.7 MB (53690855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04acf260827b0883f1ce4f6b92f0331b115421768e5cca0356ffaac834f94811`  
		Last Modified: Tue, 23 Aug 2022 02:00:34 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:45ef29c2790182012d00dae9dd827d058a6fd68f42c290ebebe458038bc68243
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56012831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d67c9769fe692d62fdd0b82c86279bf75a02daed41bd5031ac4b35acce4db2c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:04:04 GMT
ADD file:718525d7041ff4b05a60d23e77526cebc9f1b62915e7037d43558e579f5639c7 in / 
# Tue, 23 Aug 2022 01:04:04 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:04:10 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a36b3bf017cfe2e2756db405980ea7d3b435ef2a1eba38e958b5ff8b7f06f9dc`  
		Last Modified: Tue, 23 Aug 2022 01:11:00 GMT  
		Size: 56.0 MB (56012605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b2e0ca117559ce735210ace40c22e5db70dbf301ae62f0acf52158ddc85c01`  
		Last Modified: Tue, 23 Aug 2022 01:11:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:18a313441151e284921b989423c23549c7392422ceb9575fe2e137ec8632b00f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53273243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2285b7b159e6be701f33d3da71a027868c38b059f65b264ad12a622702b239e8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:57 GMT
ADD file:f111219fa55c5df38672bb7b42040526beb6baca250e4ad4ee724c1a9090f961 in / 
# Tue, 23 Aug 2022 00:13:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:13:17 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d3836c0ff2a3ebbcf11d16fdfef0948db59cc812e579ab311b2e3b198b373427`  
		Last Modified: Tue, 23 Aug 2022 00:21:30 GMT  
		Size: 53.3 MB (53273019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93507289598b4214668e787ef501a02c71d8721717fcfc4b2ae725fcf4a8af93`  
		Last Modified: Tue, 23 Aug 2022 00:21:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:a6ec25eb68eca4f66ececfca129684115b4e0b612f94b07f76c87f31001c1adf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58909370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ad47b147e8ea2bec49a3627887b7ecdb3c2a432b6eb46bc938e55a359b58f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:43 GMT
ADD file:f474fd83b474b41171768e552a1993f3b7da37a522012724f0d46c2f863e8b82 in / 
# Tue, 23 Aug 2022 01:25:46 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:25:52 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a4bc0955a358c8291f574ae20699fd39fa4f20a382cc3bbdd6b74f39d40534de`  
		Last Modified: Tue, 23 Aug 2022 01:31:52 GMT  
		Size: 58.9 MB (58909148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c89325e1696407059cf407349030f0706ddc97cff7ee197388507b4e9e7cabe`  
		Last Modified: Tue, 23 Aug 2022 01:32:04 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:e8e297c7834c4d1948bb05548ccf06287969f3f6a8802937b9b8fcfb0b46fe20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53265038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:366792733fcf4497889b5c94a5079efdc85be55e8417ef26e5c7d8a60290c155`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:42 GMT
ADD file:10e04dedfed81a283cdd807d30be507c7e18a597e0b6e6046ae1ee607c85dc26 in / 
# Tue, 13 Sep 2022 00:48:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:48:51 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:65e855ca2ae8ffaac40847c62a164755b2fdb4cd855c7fc502c00c7c3ec746c7`  
		Last Modified: Tue, 13 Sep 2022 00:53:19 GMT  
		Size: 53.3 MB (53264817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3f45a0c6770ec197023bace2187f00c99749031c21b578d33102dec028bb0e`  
		Last Modified: Tue, 13 Sep 2022 00:53:26 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
