## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:d77eeffd24e848a1a1a7439448dc2a6fbff2b02d7417ad98f5f3538a3c940ecb
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
$ docker pull debian@sha256:8bbc42e241991c1d704a7d99a52fc259503f3f8d23b4eab0c1b2dca1215fd4a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50858800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6428b8140abf71fa568981a522a9996c9798f94cf4e0ee3e544707911fa8f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 02:04:14 GMT
ADD file:c295ac949cf6eaba5c5d52c389db08bd675e330909eff8ffc4830f470e00e191 in / 
# Tue, 31 Mar 2020 02:04:18 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:04:31 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c022ee991294966f0839f32cefa09d5adb5a31987af7b4230925f0d6dac86599`  
		Last Modified: Tue, 31 Mar 2020 02:11:13 GMT  
		Size: 50.9 MB (50858572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3432200658758cbbdab17ce28ece86857654b1f89fa92a02c1e3cb25c8130c`  
		Last Modified: Tue, 31 Mar 2020 02:11:25 GMT  
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
$ docker pull debian@sha256:8800bf3f24a7ba87382a4fe1a3e63ba0f0cb2c02f802733607ffa904798c7ce6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55810526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82e38b491e1c464f08c9d37dc41356afe0191888cc2c82ace33c1cec1c97d6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:30:51 GMT
ADD file:544f960bbf6b0c556a3946247e7163ea2d8976c01f513bb4e7ed8eb8df4d09ae in / 
# Tue, 31 Mar 2020 01:30:57 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:31:17 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:de0d878984bf9a338e5828a66a5f63ae0852a3a1838645e030f18c29df6748ed`  
		Last Modified: Tue, 31 Mar 2020 01:42:06 GMT  
		Size: 55.8 MB (55810298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda045fff0ab689e028beac81f8b832b2b09b89630ee18c0524bd110a2e9bcc3`  
		Last Modified: Tue, 31 Mar 2020 01:42:19 GMT  
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
