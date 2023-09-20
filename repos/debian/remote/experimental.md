## `debian:experimental`

```console
$ docker pull debian@sha256:ec7fcd82eae88155d9f7c56e4eb95a867618960152c481d25f6e514940164233
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
$ docker pull debian@sha256:1645ceff86b47e72c07daa9cdb901483801e8eaebb45ac8cdcf9b7541ff6118b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49492551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08107bdbd0a97585dacbab12f9a074b7e131a674316ebb7a6ad41d6608ff551c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:23:48 GMT
ADD file:25321c7af80a4e7101b4d24bf4cc8940fb66ae7c55458b7d296a9a2131fe0e63 in / 
# Thu, 07 Sep 2023 00:23:49 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:24:01 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2f17621e3a810867686957185359d2a7c87cbdb129918ed8183d3c9e27ad3b60`  
		Last Modified: Thu, 07 Sep 2023 00:31:02 GMT  
		Size: 49.5 MB (49492327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df36cf06273bceda05bcf4b08e408a70a94889744145af66bfcba53761495a0d`  
		Last Modified: Thu, 07 Sep 2023 00:31:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:238c202e5e07122d00f19c305fb64f11a1bb4fef6c5d3a1a89488b7050a8f98b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47166110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fff5d12d0cf3723b278c28a516acffa97a5c604936bd81e7c829fbc500c4890`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:52:49 GMT
ADD file:efacb4b54656a7d70efa5581608c5107764d5c325ef3525f20da886cc9d2db15 in / 
# Wed, 20 Sep 2023 00:52:50 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:53:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3ea5112c05eb52a1a7adc2e1ff947d9ef11dd65aa8db61d85f145977de37d94b`  
		Last Modified: Wed, 20 Sep 2023 00:59:38 GMT  
		Size: 47.2 MB (47165888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fa3e57da9074002184c9ddd5e1b6b880d33e866055f1ff4e8bf97f1ed879b6`  
		Last Modified: Wed, 20 Sep 2023 01:00:06 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:b8728286de301dbf299c5d8734c10ad8e326f63733a63b68ae7716b520020402
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44983468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48b76b97877120c7b3ee91bccdea0f9015af502c1052f608c145d4c09a21c512`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:00:46 GMT
ADD file:46be9ca20a5324b408a03bd189ce5f603cb38ac5acb31d2e0f0f48b9d33d13bf in / 
# Thu, 07 Sep 2023 01:00:48 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:00:58 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:17d68d74ad7d056e02ca94bc23c2bcaf7137006f23b9500e899bde57a97ebd0e`  
		Last Modified: Thu, 07 Sep 2023 01:07:26 GMT  
		Size: 45.0 MB (44983248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d831d3e14dc77e99ea9d0af3f347df4ae8184182d500d86a1c9aae60fa6534c`  
		Last Modified: Thu, 07 Sep 2023 01:07:47 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7d41dbc78403eafdcaacecaa2324bb60ee6a01cb295246be9eb8cf45ca365aae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49413296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62e6797999fbd414a6f9087a735399c2c63319e779a472b8d8674c95587efb76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:37 GMT
ADD file:6a09c7783dc28deae0fecb9a5c9cbeca8ec7eabf8391afa4e37c4e49f680094c in / 
# Thu, 07 Sep 2023 00:41:38 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:41:46 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:86766b7cc4b95e7b32befda454457cefbf834629242ad14eae4435d6acc4e4f6`  
		Last Modified: Thu, 07 Sep 2023 00:47:34 GMT  
		Size: 49.4 MB (49413077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84410c66ab44715ae983972e7e6227fb848341ab8e42af421fd2c56fddfac6a7`  
		Last Modified: Thu, 07 Sep 2023 00:47:54 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:2586381086b7ba3f454eecd770fa8b24c681d0dabdd14f9b4277085a9b7a30cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50483356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58bd669e2db5cc1fb364d2b8e3e5bd6f318c0da3770d12b366481fcd8de0f9b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:45:00 GMT
ADD file:3bb4d051fa5479e355b15385abeadbfa837f0821c7bb7deae4ef60cdf97a818c in / 
# Wed, 20 Sep 2023 00:45:00 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:45:12 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:68e4fd76cb5525e54a59b89c74b172e28043f1983c094aad05f784f90f3b67d6`  
		Last Modified: Wed, 20 Sep 2023 00:52:37 GMT  
		Size: 50.5 MB (50483132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a9afcc3ec989f19fd54d38ea92d23b13f7eb0a710358015dde31ed56a53cb6`  
		Last Modified: Wed, 20 Sep 2023 00:53:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:d7797277577fcde7b65cd9ae6d01549ea565856155dfda1afa16ab7135dff7d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49338162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f837da6e6efb3e85398033e8273e3873671b8afeaf834a50565473249d163b8e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:17:16 GMT
ADD file:cdb5227ca9888541f94bc7510e0f8ef7aef51d16343683a49d0ab0982efcc5dd in / 
# Thu, 07 Sep 2023 01:17:22 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:18:00 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:78aba6dab7fb47f7bfa2eed3fbc3df39c96e726c6d64ede2ab886afc7924281a`  
		Last Modified: Thu, 07 Sep 2023 01:28:26 GMT  
		Size: 49.3 MB (49337940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7aec640e50df15492daa181c290bbc3eb4fc9a2bdc9f82a3577ffa660a9ae3b`  
		Last Modified: Thu, 07 Sep 2023 01:29:06 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:4b30d009b07f0bb66aec3a388b4d792e297fce4e3fcdb246538ab41ba6167930
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53430049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3f8143cffd39b692b1b7dbe756b6e8fb57fe74b946c192f7473a5f2eed617d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:28 GMT
ADD file:689b71ce1e06732939c4a9fd605f01bf0c2bb0a103a6e8ad2d628aaf3957202d in / 
# Thu, 07 Sep 2023 00:21:32 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:21:51 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b7956b481f448c7c033428e86a46af1c78240a8b8bc6d641e8c9770f7a239f27`  
		Last Modified: Thu, 07 Sep 2023 00:28:36 GMT  
		Size: 53.4 MB (53429827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba777a92cf8d88bfef717f2b48875c502bb9d9733bcc55ac9f7536b1a1c90a7`  
		Last Modified: Thu, 07 Sep 2023 00:29:04 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:e08fca1312c295ab8ad2841f4ed6e36de03309c233d3051874170ab4a7ae03f1
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47886230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc784227faae7baba952fabcb31d5132bea3cc613402980652031e499def33dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 01:11:45 GMT
ADD file:6a9fad96e58d832f0ec36c085b5b9904ae84876ad08531f6c3c132d3be73dd3d in / 
# Wed, 20 Sep 2023 01:11:47 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 01:12:21 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b0c261248d3418f436857a29cba81500d32de6cb99f0dec9332afcf0a92999f4`  
		Last Modified: Wed, 20 Sep 2023 01:14:55 GMT  
		Size: 47.9 MB (47886007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10557eba7c5e511a82e3ea746d3521945b345f619939bed42516bdd75805b5b`  
		Last Modified: Wed, 20 Sep 2023 01:15:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:f154abf54eeaef9ddf3b08cf0dc9d019a7d34cf4caf81e060412ddb9b84c718d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48730661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0595e392a1e38df25ef8ae3b6efe126847650d60893e511c2bb89a9b1ac1f41a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:47:54 GMT
ADD file:a6cd1b3b8d7fb4c2910b8f4a940d79edf6f736f573bf58255fe9ccbb1a7061f3 in / 
# Thu, 07 Sep 2023 00:47:58 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:48:15 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3c8dc08a2f406ba73632d434d94ac4abd2464b5b233243953592e3077768bd83`  
		Last Modified: Thu, 07 Sep 2023 00:52:44 GMT  
		Size: 48.7 MB (48730441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a3d39a2769e8eb55d60b3f6512ebc5dfc48ee2b472d51f8bfeb559e36971a2`  
		Last Modified: Thu, 07 Sep 2023 00:53:02 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
