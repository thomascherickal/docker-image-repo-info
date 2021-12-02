## `debian:buster-backports`

```console
$ docker pull debian@sha256:200f81ccdd505381de8d7b9877301e87d6f2f9ab71b8726b40777d1478f92a69
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

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:920b0d09d34851bb21cad4f4add43cd574f0c05b715f75dead7a6dbb9e029aa1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50437336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033877fbfa83ea1bb724f520ce17254cbbc2d75e7a791b8d18132c71f40c5f38`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:48:36 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50d341b18272ce30c5b682e151a5690faf0c9b413c2035bcbdaffc982dee1aa`  
		Last Modified: Thu, 02 Dec 2021 02:54:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:ad4c2d9058390ef6b06729b5a985a0e04446ba696b4a43b241b045eb18c5559a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48154543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b427c064eae13605fbd26b658d9d2e84931fb050325eca4cfeb73849ed180494`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:04 GMT
ADD file:8bb721dc246dd73e2e3ceef5631a3d18a8e9e9b00e27322673163926e103af48 in / 
# Thu, 02 Dec 2021 02:51:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:51:23 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a1593bc232eeb9f23957084e12e8d4be6b14f8a99d43fd93b74963cfca9a24a9`  
		Last Modified: Thu, 02 Dec 2021 03:10:08 GMT  
		Size: 48.2 MB (48154319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b6fbf30f1d4491c6498327b7a536f9145510f5b1b93c82e9b153a91fe916a9`  
		Last Modified: Thu, 02 Dec 2021 03:10:30 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:7a6c0e52c73944eeeebe84a21fea693d20a9be36311c6c5d6e8fca6f86e0e9f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45918350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e24b3dd556af5482d6bcad1786f911fb5b0eba2d4c046dd7586765b4bd494ba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:46 GMT
ADD file:f81ac7bc8750cba292278c6c9352e694325534f013022ec41fb4372853425a20 in / 
# Thu, 02 Dec 2021 09:05:47 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:06:02 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2c5d3a36ba44675d774d996a47340758fe658760807ada03e875b485efd98631`  
		Last Modified: Thu, 02 Dec 2021 09:21:46 GMT  
		Size: 45.9 MB (45918126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24406a674dfc4a4b68b87fcfb213e7a973b66744e296634a482d3b775cf2d36f`  
		Last Modified: Thu, 02 Dec 2021 09:22:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c6c5f2dc0f56dca0ed5b6cead8c67f938dd03dfc4d0d03261c4846c7d65f5d90
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49223271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e3726f223ce54653ed18ae4c9274af4bd34f9e04163362fa6a9deb6ead9240`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:08:27 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e92a9b4d30913e0dbf19140c720a9bc13d27aa29581258fe8dd787e8ac7a24`  
		Last Modified: Thu, 02 Dec 2021 08:41:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:2178d4ad75ead315626b3a21b46a8933fe2841935bda823cdd97f527044fd11e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38e73a26edebded63c9f2a62cd79b37efb958164842a7348d81047afb4449657`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:08 GMT
ADD file:bc6354e2db2c2d7e91d408526595618af60bda4ed24c3669f5cea44654246a02 in / 
# Thu, 02 Dec 2021 02:40:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:40:16 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3ed3f8c8d2c596bcef8beee90c4666003f0848cc4a23aaa9a695092c1c5da63e`  
		Last Modified: Thu, 02 Dec 2021 02:48:30 GMT  
		Size: 51.2 MB (51207683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e1c9617f9d674ebf17b46dfc6374951d1fec856123ad6a0bd6e173de12f277`  
		Last Modified: Thu, 02 Dec 2021 02:48:47 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; mips64le

```console
$ docker pull debian@sha256:6ba7e2f1d63f603ebf990a05f4feaa8859beca50051c0f880ad980ddb24170eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49079698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d86986b19571a34c08170a6160a5ca29968c71abdbf41a340782cdbbf3be40c8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:36 GMT
ADD file:095248cbc68568fe0013b4326eccee4814a57b1d78090c33b74fd9411ab2da06 in / 
# Thu, 02 Dec 2021 03:09:37 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:09:45 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:db00aa5bb460f25028e8f1293b6a9fc4b7a63ea0c2601b0b4e6f8b9e5acfa683`  
		Last Modified: Thu, 02 Dec 2021 03:18:43 GMT  
		Size: 49.1 MB (49079474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a73ed7646f25350d1d939c1a667a5c4cef072d82f26b33eb499ce74a4c7a9af`  
		Last Modified: Thu, 02 Dec 2021 03:18:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:7249ddf4f4b949329cea46d343b5b7be223c3c476b5c320050217fb7e629da32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54184008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d9f96f5e7a999ea837c017d7f4d5e793fd2ebc2292b99aa367be4dd2147ab6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:40 GMT
ADD file:57b3fb8e49c4d437559f3682edb29b342dd97e4913269a33c178d9eadbba9abc in / 
# Thu, 02 Dec 2021 07:21:47 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:22:00 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e863e86537b5fca0c122c393c3cc05bd29095cfe10c60ec14e3024f0589df622`  
		Last Modified: Thu, 02 Dec 2021 07:32:11 GMT  
		Size: 54.2 MB (54183785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90011f95bbd10a3c9783f048298d7f2207bc72fbaaa01231803f83c473596af1`  
		Last Modified: Thu, 02 Dec 2021 07:32:28 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; s390x

```console
$ docker pull debian@sha256:f4cfe71764820a7ed5dab18398c3cbcffa74aaf57550825d3f9fb8a58d37ab13
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6286c9cd7c9c594c5a2fdd827ee4bcd9f352fed2dfa842660845ccfe326955`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:20 GMT
ADD file:4db1e9d86bcce91ecfc6e5ee0301fde6185775dad4c6b2e0a20737e935afee45 in / 
# Thu, 02 Dec 2021 07:19:24 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:19:32 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:880071943e5204965576e16f73b7be79cd355b6dfa2808413019623a4fc50be8`  
		Last Modified: Thu, 02 Dec 2021 07:25:29 GMT  
		Size: 49.0 MB (49005485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e64d54a425829bdf40c1dcd83af4b6074d8bfd37583dc24bc86aba735862bf`  
		Last Modified: Thu, 02 Dec 2021 07:25:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
