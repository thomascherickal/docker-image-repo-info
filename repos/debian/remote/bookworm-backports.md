## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:45d34d30a8905c5b0046380cb5280bb1f19c942c322804b8e2b9f5818a477f55
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
$ docker pull debian@sha256:b169c2cf97898d33cf0f9732643f2ac049f411fed455e883e0b37b3d4f5b31d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49551656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e7e3eb1e0ab9997e94765d06a353aa08d455dc2aa0b161392335e88fbaf8f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:19:49 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80682bca8042a81d167d26bb331b9837b042d8d1934fc707b744f04114ac94a`  
		Last Modified: Tue, 04 Jul 2023 01:24:53 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:685905ae2de8df0c3e164a787377af1585e3630ca14007f00d3f310bcf55e718
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47403011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0f960c2e7c48328c1def5b6f4b328a7ee2778738ecc2960146f2f624e24fc3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:48:26 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111794510e313108d92691330a5947a9996ab861b2c970b2c4423bcde8605172`  
		Last Modified: Tue, 04 Jul 2023 00:51:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:3fafd6c274b0fddbfbce6fc9aa88c783c6202c5575d526fbcd2ef8af25af65ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45236426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d047ca742e5a12c251806d3e8c69340d31602c584cb9b4a947bd3cf0a81baf6d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:57:46 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6558e9eb6646f3cc0af1052a3a9f2ed3a88e5a3e33ad0a806ee77d857b26dc5`  
		Last Modified: Tue, 04 Jul 2023 01:02:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:69ae4ad0bbc9a1b250eb52d121deb1044e557643ae767a1d3624b881e51b1ad2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49573385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f105379ab5c2bdb5d89e566866265674b704b61ae3891f9ae46aa0e223b2b9bf`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:59 GMT
ADD file:0dfaa4beac7b0a95f2b33bc35e08b104057469f46fa35df2af7193451ab3714d in / 
# Mon, 12 Jun 2023 23:40:00 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:40:06 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a31111d070044ed920abddebc16bfa67a69fb0e0e782b703073c93ec10dedf67`  
		Last Modified: Mon, 12 Jun 2023 23:43:47 GMT  
		Size: 49.6 MB (49573162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2404e3e5033b0c75c36448742c96bbb287b8d8c574fcb4f91addf5c157bb65c0`  
		Last Modified: Mon, 12 Jun 2023 23:44:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:e6e10e3fd289c18cfd914da4c2c9e2f0704c27ab46bd1a28d43d1847af67d519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50562616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54e28f469bd1a222790fa4a3a6fb86b81694a7f6e6c54f1381b47add364f9b5a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:02 GMT
ADD file:a0aeb9b361b31d75c8d96223fac8f3df2807735ed20715b24af45a414ad3965a in / 
# Mon, 12 Jun 2023 23:39:02 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:39:06 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b9cf3331eb07181e9e59fdcd7e0dff8a268c9d12151911a49cf687e8007305b4`  
		Last Modified: Mon, 12 Jun 2023 23:45:56 GMT  
		Size: 50.6 MB (50562393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58e606fbbcfee46e1da61b2f577f0a0875913a7ef78bbcc19c16b8d34804ab`  
		Last Modified: Mon, 12 Jun 2023 23:46:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:25cdd4baaaa2a8d2969a6e492f6732a791f2143840fa9be951eeb49a8c46cca6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49542369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ffb6186eef8eaedd3436861ddef5b97f7af46d4978fc0fbbec8abdd03e6ceb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:09:05 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e06f7c231fa5a11cd333646ad54b7a628d8cceb2ce48842ba9eae85d279a6f`  
		Last Modified: Tue, 04 Jul 2023 01:19:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:56e56a9923f2c480133f840026f3389c29322a42055e51c8cd09632b670da4be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53536966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f14b6596252a15653fff7ab47831720f0e960ad7fd708e055b4314ea3bce74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:17:38 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03702ace77d8f2a14b0beae6a5a330dc8271920848ce13a7ace1f7ee85636e8`  
		Last Modified: Tue, 04 Jul 2023 01:24:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:30fe7b063f3d35cd75fa2fbce94fb4e92cf6d94179985d65f34dc44d3aad984b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47921819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dee92e2bbea2f07ba73786aa19ddbbc7f0326d5e3f4a6798d648560968bd7862`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:22 GMT
ADD file:249060834694c2236703705d65a79827f5e97ac9cf82b79a6941cf0f47134556 in / 
# Tue, 13 Jun 2023 04:29:25 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:29:32 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:568dd23e2b461377b9cc9f517f959ed366ef5f337dcef4396672fcf62e6cdc68`  
		Last Modified: Tue, 13 Jun 2023 04:34:06 GMT  
		Size: 47.9 MB (47921596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0618347ddc2b9f8dbf07011175baf2d63da6b478ad0fef0991bb267a02f65a8d`  
		Last Modified: Tue, 13 Jun 2023 04:34:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
