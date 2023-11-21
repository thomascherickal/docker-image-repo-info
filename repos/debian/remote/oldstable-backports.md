## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:98f1b13b5e567fd066a5c5ffd4b68808c19d9942eff7126906cbf10ea4c9c7d5
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
$ docker pull debian@sha256:bebd18bdf6c6fb1392e424f8b8ab830d69b3d09a41af3bd74773c93545372678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55058322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc6988002241c131bf5fd8a90ba323a99dd0eada326e0d1f5911c22e6c2139f4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:06 GMT
ADD file:30b9dcfcd946b137141d7c5c2edcb9d0817dbdd07b9a6951031ee071ca2e2894 in / 
# Wed, 01 Nov 2023 00:22:06 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:22:10 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:41bc806f354b99a3f6009571ba6c37f6532fd5828fa506fd50fced3b011f35b5`  
		Last Modified: Wed, 01 Nov 2023 00:27:52 GMT  
		Size: 55.1 MB (55058095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cad93d1666898656190584faf83c3f1f4048c7f369d01c5611d678be153ea67`  
		Last Modified: Wed, 01 Nov 2023 00:28:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:107ae6ab66ca50288c9b2e251b62f6184fa8ffc6878524320868204cb48a3c01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52563125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c4f250664fcf223bb7f9d27709a0110255685d345bef09f0a173f5c6d39efe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:16 GMT
ADD file:f36fad21c34f7be5a996ce7afd1ef72f359d1717caae650798781f4dce9b4067 in / 
# Tue, 21 Nov 2023 05:01:17 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:01:19 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:675c66f4e425fb4dc844bfeaf4ab55692c212d536f6fbb61083a3bf367441d3c`  
		Last Modified: Tue, 21 Nov 2023 05:04:58 GMT  
		Size: 52.6 MB (52562900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1419b1431ac1b89e35548211fcbef6ade7d664e1b8fb0c2216170d81797623`  
		Last Modified: Tue, 21 Nov 2023 05:05:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:2b9a2671906236fe840a37ee9b3399ebc9f00c53f59e3c90254e2192825c8388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50215879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4584db1db5ad37e293c8276127c0c200811dfdfdfd386837ad1da39e080b00cd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:49 GMT
ADD file:58f6f7f29ceab3d3aa9804f9f3b476f110673cbbc0ebd7d72d01e8b8089c585a in / 
# Tue, 21 Nov 2023 03:58:49 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 03:58:52 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9be29f3594315c42bcae957a357b11b71d9dd666d2deb5c9e9d10f669800d5ea`  
		Last Modified: Tue, 21 Nov 2023 04:04:19 GMT  
		Size: 50.2 MB (50215655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667c9c92f823a45a648189d0c653102db88bf427e2ee58d8abbbb1d0ae63cecb`  
		Last Modified: Tue, 21 Nov 2023 04:04:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b4e66de73650741994fa0a96866507ba78ff61ff62916ae88dc3e3e74b052d23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53707947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef88b7ede14f1b02981a25143b093eac9423fa6eb3b7e832fd16ccc1491fa98`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:b30a343af65c645e74d2553af6919092522cdc54756aba1d0adbfbd0d7d5d4cf in / 
# Wed, 01 Nov 2023 00:40:31 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:40:33 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cb543055d2e84a942c853542b1080a71cdc776d4f28c8eafbf2e4fa1ef2759ce`  
		Last Modified: Wed, 01 Nov 2023 00:45:14 GMT  
		Size: 53.7 MB (53707722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7685f69d05bfee11937fb0a53aeb56e2868043a8847529bddf0b7b741acc33aa`  
		Last Modified: Wed, 01 Nov 2023 00:45:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:17cb9598226812adad07aeb32ae3bafc22a6f8a11d75ae0b4feb6ae806a9dda0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56046522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b772eb6d1e31f534818c317df62523e6cd11cf88303f7925dfee70a6985ce02`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:41:10 GMT
ADD file:217157e9134f1fba9dd152bd3f5ad2b1f198f34364ccc53df7cd2201a970eab2 in / 
# Tue, 21 Nov 2023 04:41:11 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:41:14 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:748f1dfc0d9b0fe114ab94a1b33ec19aac61d62b6003a98d6b32c9339c150153`  
		Last Modified: Tue, 21 Nov 2023 04:47:12 GMT  
		Size: 56.0 MB (56046296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42b4b154cc4f9c7eb0f0fddf26551ce4d4ccb3de11a3923342e60f85365c520`  
		Last Modified: Tue, 21 Nov 2023 04:47:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:05abf1f379cd5f45399a0fd1ed99ada1e9a5e6a638e5e95cd2a0591d8f75e435
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53289388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd31a12e7921faeb73b8175d183cd8a8485bedd5e9651ca9c31b8bde9e12adca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:11:38 GMT
ADD file:343c03861fde637104bb6e0f9fe190e9a9241fd256235e98d22b6f3ecd50f018 in / 
# Tue, 21 Nov 2023 04:11:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:11:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:01df819effd0b4438405ff3eccbb77832cee643b4bb690c24074c16314ec0db7`  
		Last Modified: Tue, 21 Nov 2023 04:22:45 GMT  
		Size: 53.3 MB (53289161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b451372d0365100d5e075c3e7955e886215372a4feaa1cb6c4963e8b0c9ceb3`  
		Last Modified: Tue, 21 Nov 2023 04:22:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:fcd6c470d1f6a16dc266a4573785efd0402bcede9ccc375ba5843e0c9a97c2a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58929916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40507bec850434327a56f2c59a467de523b508cf892a0770ff055561306ab34f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:57 GMT
ADD file:74a569df19366491efdfa37a67b8b7f950a1a6f9ffb9ffd83ad6e00e83113417 in / 
# Tue, 21 Nov 2023 04:25:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:25:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2ab175c1db3d58863ec0f724c79351d3f9a9c2265671417eb42ca94f686d3838`  
		Last Modified: Tue, 21 Nov 2023 04:30:09 GMT  
		Size: 58.9 MB (58929689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a247d1cf2717f871c6769dc23ac5b29754aa0a9c888ac3d73b7948890f9a55c9`  
		Last Modified: Tue, 21 Nov 2023 04:30:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:f4cd7cdf8d55085d55be3cb3a21cb4643ccc193faaa49edfdda02757e92d2ad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53296634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbf802d266052128fe73f201dde75063d6fb93e076284554eba2a6e9120f65d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:33 GMT
ADD file:69c3852647fb10851d4ddd10673e49616483b349561b50e5f4faa8c2f133326f in / 
# Tue, 21 Nov 2023 05:05:38 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:05:45 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0637dc42a42394ba3bca511cee58f8de5e1410706282b8b69d3e8eb31112ca10`  
		Last Modified: Tue, 21 Nov 2023 05:11:00 GMT  
		Size: 53.3 MB (53296409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781a060e7c00abdb28f4e5bb3d469723b87f0a31e458798beac574c3b19606e0`  
		Last Modified: Tue, 21 Nov 2023 05:11:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
