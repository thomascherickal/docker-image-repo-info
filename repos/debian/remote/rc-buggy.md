## `debian:rc-buggy`

```console
$ docker pull debian@sha256:991c6d84957d20b1544d7b38193c6900119138a12eb307176affcaa010204e31
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:d09fc4f45950e974951908727b62c43c0aa1a7499c31de0ce66189e60e137785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49234740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d73bbfb183273ef3e56c0958749bcafd9389d954c2ef6a1b2d9b8758e469ced`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:29 GMT
ADD file:b3a4ee0f0fbf2d8fbbab0aefd91aa4d658c41b09c8a2beea1024bfce5e7d3fca in / 
# Thu, 09 Feb 2023 03:21:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:23:10 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ca2c7deeb5af7aa8a0aa3358218901c07b10bb98573151782e5e7af0ab03009c`  
		Last Modified: Thu, 09 Feb 2023 03:26:46 GMT  
		Size: 49.2 MB (49234515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d558964e37f3e4ce4580e72806504565978a967b421897339aeadd0cc4797a2`  
		Last Modified: Thu, 09 Feb 2023 03:28:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:2f4c87930a8052854f1f0a419b4f1a6b87ea00215f8c29f905364ad62b76a67a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48168880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2dbbf3dc05c99742fe1e5dc0423778d4121aa6c6e430364b302f0bca1df8673`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:45 GMT
ADD file:dc28e6a68656b2258d74ca814eedc70f45b8b6c604f68add2cf2f5f7bca2b675 in / 
# Thu, 09 Feb 2023 02:00:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:02:26 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:cfc3c8b7a8637963e4e7c58d3159378d2dbbf0ac34f355b8781c04894e7b070c`  
		Last Modified: Thu, 09 Feb 2023 02:06:07 GMT  
		Size: 48.2 MB (48168655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612f453206de511c8e331473db28fcc8b2b8ae78780f59a3703fa2cda16b00b9`  
		Last Modified: Thu, 09 Feb 2023 02:08:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:1ec8e99193f98319694044f07e370257c819ca0e2fa46c9b3689189b7ee2ee69
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45796246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ff14e13c540c2242c660c1be078f346f964dd5e653f88e94d0955e293c5625`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 10:00:50 GMT
ADD file:3ef0e7784a31367bd6b8f62d72fd921e841a63c5f468870ca51cb13d32a10c98 in / 
# Sat, 04 Feb 2023 10:00:51 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:02:41 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4ade7fb7e5df21b5001435afddae5270817c5e2a665e698f2b89244410fe9cf7`  
		Last Modified: Sat, 04 Feb 2023 10:08:21 GMT  
		Size: 45.8 MB (45796020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e18059396a57f39fd2ed432192016283a24ad3fb9a843c3b713fec60c01d89c`  
		Last Modified: Sat, 04 Feb 2023 10:10:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:409df33715ec7cca8fb1f9e842a71b5b45a52b3ef19cb511fc1129c6b66fc48c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49272488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf2bf76dd577277f5e89f700ab575b875870e9cd39d82f473dbc875f1c828ddd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:59:27 GMT
ADD file:e092144c3667bd346dc4cb05da5a70ca9f7303d7160f9d5763af88fe51e02f66 in / 
# Thu, 09 Feb 2023 03:59:28 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:00:36 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:00f9d2ac5ed56c16a45852afb781f7257c58125a3b154fa75d18141566291f9f`  
		Last Modified: Thu, 09 Feb 2023 04:04:03 GMT  
		Size: 49.3 MB (49272262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ace1b894f99d767eeee9645f132b45b39de46f7ef1e99cc3362a0dc55be17da`  
		Last Modified: Thu, 09 Feb 2023 04:06:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:c80815d56c4caf2d1dee353c9e199b474f8f04d5fcd592869543d0111baf4d61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50095661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36b2afe1f71606e83e68d2b5fa3cf6dc3ad9e1e05f1367f9f4db75aaf6bae536`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:50:25 GMT
ADD file:e52d2501a6498b9d4b4b7c45345d2dd2f2fbfa7df2849d1f794768270c0971a5 in / 
# Sat, 04 Feb 2023 07:50:26 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:51:59 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:dc17d0499e93f237d6be86c3138e9cea4fd1d950920edfec3d640e8d8b6e6230`  
		Last Modified: Sat, 04 Feb 2023 07:56:51 GMT  
		Size: 50.1 MB (50095432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bf83f2c4394c22007a575f6fc7aa0e31b514aa1d43af2542a886e78782869c`  
		Last Modified: Sat, 04 Feb 2023 07:59:16 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:c109c7598b59a062f70ebda502d0b8b54639ec76468973b08e6febe9164eb639
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49094518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f148b3442b0fc390a4ffa7c9e246dbdb8d7000fb603ace70805eddf6dde811f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:50:42 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0851e3a54eef9d4f066d251f39404cb8e6972b5d6b068bcaa048f4755b5826`  
		Last Modified: Thu, 09 Feb 2023 02:59:00 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:c54e34360d791dcd741a01b5d6620d222ce42cbd0322d6c20a15d9f7b1dcc617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53052722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98566990cb544e5d2d91c082871becaa02e84223853768b415280d465a9678f6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:26:15 GMT
ADD file:24ea24099063f3d78eb81b653d243295dc4b47f84833c244197869e3675e3840 in / 
# Sat, 04 Feb 2023 12:26:18 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:28:56 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5983dd3dde0b9f046ad79781724edbc7a225d54d2fdbccc7f201d0ed78cde5ce`  
		Last Modified: Sat, 04 Feb 2023 12:32:41 GMT  
		Size: 53.1 MB (53052494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d0fc78af319d27223842e8059ee73f5279dcdb056082ff9dba0e8a2191f24b`  
		Last Modified: Sat, 04 Feb 2023 12:35:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:f83a82e51ce4b23c7d24f5f744f57ccade0eb90537efe8b6e59781115007fa50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47605761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6db8dd081e78592c06d7f90aebeec502c382324079aabe822bc3b324b964646`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:57 GMT
ADD file:2e666c175716fd02a858ff036fcece3fd5bc91959ad6e87ba5371f0e1c35eee8 in / 
# Thu, 09 Feb 2023 02:42:00 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:43:50 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3019a6e7de2300389d30ae5349430a715e5e0de8dee24a1c55adb1f7bf5c4133`  
		Last Modified: Thu, 09 Feb 2023 02:46:21 GMT  
		Size: 47.6 MB (47605532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeda4c4a5386da20831fc110218cb98e182844ce5f3c97aabf38c83be9c615a0`  
		Last Modified: Thu, 09 Feb 2023 02:48:07 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
