## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:7ebbbf35746db1d9c5843a652e9ae2d3f38f82c8410d1b7940d25220bf4fc9b7
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:8dd5996ecafbe1ac97610193235331ae1110190cfbc5dc4d66d01467ad8bd029
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55055811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9946fb52acca3fe295df9109f415b473bd1e9bd0fdf991c9fe05e6e5e6b1478c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:02 GMT
ADD file:d3d35fb8232fe43e10dc766c041fa6d6435ac21d31451258d21f040405ae5563 in / 
# Thu, 27 Jul 2023 23:26:03 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:26:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:784493098d3cfa412835581409baba2f10667893e59b83360d4e8a525cadc867`  
		Last Modified: Thu, 27 Jul 2023 23:31:42 GMT  
		Size: 55.1 MB (55055587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9e14c83f55be936fb81758830ae4d6befc9bd610fe62b24cc023f3cd840512`  
		Last Modified: Thu, 27 Jul 2023 23:31:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:8cefd662aacb0cdafd175551258963737a08bf8e8af5e486b4e7697e6d9a1702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52558370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528445383747c93fb31dffcc1e2a94d54afb3b69293da0eb060efa2d054bd61d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:56 GMT
ADD file:e6753fde0869f0f5afc29d8db288a9ce529874089560fba3f5aabf812b0fc278 in / 
# Tue, 15 Aug 2023 23:48:56 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:48:59 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:67f24ee25b6f816ab234b14c1a8f78303187fe1928975945689db3ff437614d8`  
		Last Modified: Tue, 15 Aug 2023 23:52:34 GMT  
		Size: 52.6 MB (52558147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e3f6ee751016093be369ec93a414882644bc6764ec26638c7091e314c63b21`  
		Last Modified: Tue, 15 Aug 2023 23:52:43 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:e1cb2217ec12128a2bf0d8f043e6a7bc2ec09c8d95ebf423e1777c0cfbd623a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50218774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c1a1ef97e3723bb3f6aebd783f2f70e3cc5fa46117ff57d9d25489afaaf8943`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:59:26 GMT
ADD file:d7a24eba8d49f00c4088435934f4be16ef020d2c559a54f859d05bdd5b0a4b8f in / 
# Thu, 27 Jul 2023 23:59:29 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:59:33 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f801e05ad008c87aedbfa56a853a8d47fdf7b5dc2680b742cc77606e7eb55664`  
		Last Modified: Fri, 28 Jul 2023 00:05:31 GMT  
		Size: 50.2 MB (50218549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c1c6f919b8bbb0eafaa8a8049774cfd0ef5a3711acbd4809de44b335f23b38`  
		Last Modified: Fri, 28 Jul 2023 00:05:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b7803fa646f61fab54125972f58a9b4a302f14137ecd0c8f7b895158d7caf97b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53705010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3472dd36b8906ec2cfaf698c0c1d763eda61bed5a8b35a76682583369de7255f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:46 GMT
ADD file:34a36ee946cf6f98b44632ef4bc6c0d3362d611d35c4541abd8b683957da0423 in / 
# Tue, 15 Aug 2023 23:40:47 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:40:49 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a10af57736c05ea7055aa2bccee0cf5869549bd35cbca2cc9360afb611d6427d`  
		Last Modified: Tue, 15 Aug 2023 23:45:24 GMT  
		Size: 53.7 MB (53704785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ce1ac1e56aa3475bf873cec0f775303854aa249f1767a749e7885423e8eeda`  
		Last Modified: Tue, 15 Aug 2023 23:45:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:0b938358115e756d5dc638a231847d914534ee6af7f430c8e373f7ae40b8f93c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56040746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b8a0a2d4bb699377fce391994f3601367e27c97f83e73555105036be3c0f33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:13 GMT
ADD file:be80506a012b48af460817cf4bafbce09ce49837492dadd0d729dfd35d7f2627 in / 
# Tue, 15 Aug 2023 23:40:14 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:40:17 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e47d27a26101bfcb6857b31fe3ba89e0ef8d7fd4063dc5b0e44eb1d58b1b765a`  
		Last Modified: Tue, 15 Aug 2023 23:45:55 GMT  
		Size: 56.0 MB (56040521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f5835cd4765d83b77d414a83614224f010a82012159916a39a5997d6c37b`  
		Last Modified: Tue, 15 Aug 2023 23:46:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:46622afab5aebbf9f375bebb8458464771e1f7f9b8e55b4a646c47e98cdd1fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53271167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa12f6858dea5af3a64763025df7ca44d812855ccce56ad480013cb2680ada1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:13:12 GMT
ADD file:71a75d283ef59ae2efbfd71e5f85e3666fbccd01ba9e283c10da754e25f58079 in / 
# Thu, 27 Jul 2023 23:13:20 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:13:32 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:331241b14a925146f04f0b145afd991bdbec8cf1f6d09fdce38db830eea2dd62`  
		Last Modified: Thu, 27 Jul 2023 23:24:35 GMT  
		Size: 53.3 MB (53270939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92076d43a4ca638bd0040e11da426929fad4d8d72f78aacfa62e0bde9b59647f`  
		Last Modified: Thu, 27 Jul 2023 23:24:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:682b713a57c8cef351b24ce4db01693dfa50d4d3c52d463a4bb39b371f0d66ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58927716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e8486b924ddbd22fb5b31dbe25bf2fb8751da4871e7a5e1b10859159403ac77`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:58 GMT
ADD file:ec924dbdcd458a572b817c41d54fa01ec94c123408db29504d74b0611a32ac0e in / 
# Thu, 27 Jul 2023 23:24:01 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:24:05 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ffc8d5ed9189fcc970c2f6120db280ccede96fb66fb23bf47ec8c1f64880ef0f`  
		Last Modified: Thu, 27 Jul 2023 23:31:05 GMT  
		Size: 58.9 MB (58927491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d6b8f92ba07230fecbcf93709e08d6e874b3374ea54b52e3f82d4162a9d098`  
		Last Modified: Thu, 27 Jul 2023 23:31:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:65fc66c47b426a11ac3fafeca0701b776cb7bc16b2c040ead2f4d740ff5fd842
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53290861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81d4d1798d2a13924dee715505b61034ea170fd09896db517778fb6233db5fe1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:16 GMT
ADD file:aa6aefd4db318e04c7ee34bec123fe1ad5bdfabae3dcbf3ba41b9ed515367def in / 
# Tue, 15 Aug 2023 23:43:21 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:43:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:79fd05fa321bd107f698cc0f80675f45b52b06193c08b8cf3f4fba1c1544fe2e`  
		Last Modified: Tue, 15 Aug 2023 23:48:36 GMT  
		Size: 53.3 MB (53290638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7448a9c4cb74c1642ed31996606401b04c6dfb2dff0a1269c069a6b54e1cab7f`  
		Last Modified: Tue, 15 Aug 2023 23:48:42 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
