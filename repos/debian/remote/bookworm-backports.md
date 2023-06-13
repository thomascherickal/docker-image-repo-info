## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:4f88fc6a521aaf660d11694b4c9ab045b3cd5baf89bf146ce446466271b8f609
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
$ docker pull debian@sha256:337c7ab55232126a2415cadf4eae2a917a76d66dc2db049937e233be64c9eec0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49552334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7c9b7357c9553f6271a39a3809dbc61735f7d1bcc244bd3720da3e4609205fb`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:28 GMT
ADD file:98cacc5890a8c0b29d7a2b296774428cb2268b01b4ff97a84deadcd3b513f319 in / 
# Mon, 12 Jun 2023 23:20:29 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:20:33 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bba7bb10d5baebcaad1d68ab3cbfd37390c646b2a688529b1d118a47991116f4`  
		Last Modified: Mon, 12 Jun 2023 23:25:26 GMT  
		Size: 49.6 MB (49552112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a87142e6ca210d97c45fe91448548487c73cccb2bdede75a9f60086966e0d4`  
		Last Modified: Mon, 12 Jun 2023 23:25:40 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:1aecbe300e4e5706dc4bc84e0f71f85492838c50d334b2d56dfb82a87b881ca5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47403453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b04498e8f14ecc2c1772ec3648da233ad456d1d97cfddf0fdc613536f6ea91f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:22 GMT
ADD file:501b903784636438cdb91607b6c13e72a99c6918c6d8d24620d21a6907b3c919 in / 
# Mon, 12 Jun 2023 23:48:22 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:48:26 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f33a06945c2ca0f2b7186e00c7917f40db046448f78cca610bfb4e899c54ccbf`  
		Last Modified: Mon, 12 Jun 2023 23:51:03 GMT  
		Size: 47.4 MB (47403230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348d86eb6a089edb117ef54612c2a89f8a461ca1a1d90b6f3191a421a86ba989`  
		Last Modified: Mon, 12 Jun 2023 23:51:17 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:21595686373e188bbaf67ae6c4c7886cbfa4f316630ef5f8f9a0d7232cc255af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45236395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:412d0161815fd698416401ddfa31cf673802b33f608ad880fcf236d25e506327`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:10 GMT
ADD file:3af917fd4b956bc618904ef0ee9783c26f07442cfd03eebf92634280dcd2fc44 in / 
# Mon, 12 Jun 2023 23:58:11 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:58:16 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7bd3ccf07376cd3298bc10edd37d559052da8db8b3a4329639d1f41ad9e69921`  
		Last Modified: Tue, 13 Jun 2023 00:03:22 GMT  
		Size: 45.2 MB (45236172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d20d26a54789aaec3f64177908066a7e13f2f60751fac276943a6417e00a6f9`  
		Last Modified: Tue, 13 Jun 2023 00:03:36 GMT  
		Size: 223.0 B  
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
$ docker pull debian@sha256:de83fe43260404a28b6c2a66de91bbf9c8f038117a5d1f79663d69ebfc184364
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49541761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbba8c4ac12cddb377f2a811ee131455276553232acfc7d28fdab5f5729552b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:08:08 GMT
ADD file:fbe506fea544eae98a8a13d6b55d001b4327c933053d898d5a19bf9ffd7470f8 in / 
# Tue, 13 Jun 2023 00:08:13 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:08:29 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fb5fba29e113a7ea4313a026e3a37cd5bc1425850dfd19a63973d48c89e0f266`  
		Last Modified: Tue, 13 Jun 2023 00:21:46 GMT  
		Size: 49.5 MB (49541536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8c658cbc1d852cf17473017c500f05864941ba32b1845a21cb5736eb28495`  
		Last Modified: Tue, 13 Jun 2023 00:22:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:cc1e1f6d8d6a6922b0deb2442fa889446e19e11607e40ed0b253bbf00815a716
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53536977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a24d41f1bcf3ed8967912453402cb36e2b7bcf794c43365f142aef7d08c877`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:10 GMT
ADD file:016534815cb7d12cae071da7f55250eeaff3ebdc6c1e4689e32d50df1fb158db in / 
# Mon, 12 Jun 2023 23:17:12 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:17:19 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:622cd3709abdd2a8ae1c5270932d62e2474b25e69dbd2e143ebf083f3a8696aa`  
		Last Modified: Mon, 12 Jun 2023 23:23:39 GMT  
		Size: 53.5 MB (53536755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91211e27e0236480136cf2992e15a38cbcc7446c306e9672b6a007886dcc3a9`  
		Last Modified: Mon, 12 Jun 2023 23:23:54 GMT  
		Size: 222.0 B  
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
