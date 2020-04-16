## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:f4992c8385372f8a4c57c0c4f73a78672f8500fbbf5b61e938a0aa067c660bdd
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:7a918861d75b362de95fc215845b3aa5fb2f1db3a63b360d969e1aa84d4ca334
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51922913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0f0fa6c3ab8882e11e334e5a6531bbb2da48d77259187be64cd2d8bf3f2c46`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:20:09 GMT
ADD file:edfe2fd644e397f293f4634d48f0fbdadcbf9e5d3f226da6daa213811d4bfb90 in / 
# Tue, 31 Mar 2020 01:20:09 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:20:17 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ac0531d9afaea848836097ce37941ab7f0d2533a1b6c1cec0eefed4bb8d4d9cc`  
		Last Modified: Tue, 31 Mar 2020 01:25:55 GMT  
		Size: 51.9 MB (51922687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4534143be9195563db68b0593b4e2c321272d57eac692558d021988570cb5162`  
		Last Modified: Tue, 31 Mar 2020 01:25:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:581b639d2cae349438d0c48b359478c9e07be536bd7a3f5708dfcd08d1c2d44e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49911807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cad276c5f74420a3000b58ba102170e5af8d9f18923ab0e4ed8fac425617ead`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:48:51 GMT
ADD file:34972a3f69849271a3928351165da58547b7e747a95139712188aa70c0b57364 in / 
# Thu, 16 Apr 2020 00:48:53 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:49:02 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:562c28f550656170c3977f83af3b203cf461b48e55905e20714735c0da33f6af`  
		Last Modified: Thu, 16 Apr 2020 00:57:24 GMT  
		Size: 49.9 MB (49911580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593674200e826ed19e90238ce66d4162b639ff04973bde909c5869abf0e066f`  
		Last Modified: Thu, 16 Apr 2020 00:57:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:6328a00ec3cba52c771340bcbfbf789cd631e7bfb06d691f48aeb2c18f5bc60e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47646617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fd3e5b2542428b796e6c93ad786b21a5473c55f94064031df8ffbe60150699`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:58:05 GMT
ADD file:353f89e64e5475f2d99be1c5e0eaa80d5aeb89e02c274ba507df4def8f7ccc8a in / 
# Thu, 16 Apr 2020 00:58:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:58:26 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a287a7fa81e293e147ba52c36ae34e643e975ef88ebe9a6f226a048dbb7ee9fa`  
		Last Modified: Thu, 16 Apr 2020 01:08:03 GMT  
		Size: 47.6 MB (47646389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0da0c4bd275aa4efecbe71fe2cbaa57debe09244f037e8b622a6b2ff88ff78`  
		Last Modified: Thu, 16 Apr 2020 01:08:09 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:64686de29480050d68f81f27cf225effda5400d7a7b84733f1bf9bee37e04909
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50901693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ad4642edc0d630447491e524da01c87737ef37d3ef0f34306aac551076782c3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:40:12 GMT
ADD file:27c25cdd69090f4b15f9f2f4a147879d1d7510b7b2f8c231a92fc74832325413 in / 
# Thu, 16 Apr 2020 02:40:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:40:37 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6c6bfde49c5261423574a9f9bc077a0cd0057775509f9d9e061556a16b84e1d7`  
		Last Modified: Thu, 16 Apr 2020 02:48:01 GMT  
		Size: 50.9 MB (50901465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca635a82c0d4543c559a12e05c3eaec02a9e1d51c8dee3b02957c1bf39a2d2d`  
		Last Modified: Thu, 16 Apr 2020 02:48:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:9248248d0daf6b588f92955bf3bf35a4fd2682e7a6db35b3c7e4d65c5e43cd76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53116725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac9e1c615db89e0000c42a0abae6296a9dbace80654cb9fe91792033cb3cebf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:50 GMT
ADD file:1d78edb74644d640409b64831c000f00654603e8888b50c46ac37ca0c186c3e9 in / 
# Thu, 16 Apr 2020 01:38:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:38:56 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d162d6311c3b7618a8b9a80392bb71455272c7ef63938e132282070923f16ead`  
		Last Modified: Thu, 16 Apr 2020 01:45:26 GMT  
		Size: 53.1 MB (53116500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e1e866c8903963fd81c76bca4bbe02a9dcbf15874463f721f03fd6402808f0`  
		Last Modified: Thu, 16 Apr 2020 01:45:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:ee846f87be0a9bc6a16b5697421768b4c462f5c0a1569073e7b631e2e78a8f74
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55848342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e67446c9ca2f77547733ad70b46bd6208ff0d82cfb9228a5943ff69af1b019f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:32:12 GMT
ADD file:2efc2c0f69b08c32feb2685a63906c73b19fb52d2b93f97e10252433820bc5da in / 
# Thu, 16 Apr 2020 01:32:20 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:33:22 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5bebe00a0631d47861daeee3fc26571ca333821c566ce1b711e981ca7685ea53`  
		Last Modified: Thu, 16 Apr 2020 01:50:59 GMT  
		Size: 55.8 MB (55848114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e730a62fc622c02da0a5cc38353a9a8a339661a7acaf387fd0563cec02c9401e`  
		Last Modified: Thu, 16 Apr 2020 01:51:12 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:c10e8549eb6995194a192e94ca6ac8083dac68e8fb655063648d8f4b5392809b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50569264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa9c453996f5339ba76252c74ddde1ce74f2a8bd3607ff27dffe7feba4fcdbb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:41:36 GMT
ADD file:91904e1cbd0660c7c48420aa34dd58c0e8619c69afe6c1412a495c364773b5bb in / 
# Thu, 16 Apr 2020 00:41:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:41:44 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:929a8c37dff5f4096f453d7847637ff8b3e3fa702bd1043408eb37af338237d4`  
		Last Modified: Thu, 16 Apr 2020 00:45:37 GMT  
		Size: 50.6 MB (50569040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76e48bacc7d91800744f801e123c74390932f81f51803457adca90161b1b98e`  
		Last Modified: Thu, 16 Apr 2020 00:45:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
