## `debian:stable-backports`

```console
$ docker pull debian@sha256:c7a811e86d0929013034ad4ffe9bd50cf3c600d2fe7026eaca474f1af8f94f7e
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
$ docker pull debian@sha256:3d346fb3e94f9cf4743bcb523682a98ccf45d066098d3e33e99c06af2f4c6a1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50435824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f95fb6e410aae258f9b67415e448f433ed12c605e53a2b34fa92c7a592ab63`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:46:41 GMT
ADD file:cf0c060f55b6c6904f0b8da3b85e22c08828aba6b957ee22dddea39575f666c1 in / 
# Thu, 22 Jul 2021 00:46:41 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:46:45 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:333f3bd151deae1c6a99ac8656bde89cad36f58317dff636f1a137777b22bc4f`  
		Last Modified: Thu, 22 Jul 2021 00:52:07 GMT  
		Size: 50.4 MB (50435600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4eca13d185f1ebcd36925e2b7fc07a5ab494ef6138c37872a798fa642f505e`  
		Last Modified: Thu, 22 Jul 2021 00:52:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:7f5e497f3fcb70c50152b6e5bf3217395ceec21ab2f49830a0d3665492e4c5f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48153474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3147152f60e647e2efb4a41ad545bd29fc7680162446c49e3f9a98b2b140cfa8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:52:10 GMT
ADD file:f3d7275062c305b42debf8dfb48fb5f7687526caadc936bd39be78ae659a8085 in / 
# Thu, 22 Jul 2021 00:52:11 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:52:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:21bfff09e1240faaf3850f5e2a8e7974e604b2ee5ad6e2bd6b1be5c63e2ca611`  
		Last Modified: Thu, 22 Jul 2021 01:05:23 GMT  
		Size: 48.2 MB (48153249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9633d3d1bd6fead031cdf0d43bcbe628e65b1e1a9dc2a0f8522009b1dfbcf48f`  
		Last Modified: Thu, 22 Jul 2021 01:05:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:49ed45085680a69d36c250586e03a84923add35ab77c3fda25f3dae663825dea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45917467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cbb0733e0193686872c35a9d07213d44938d9d1888684dbced3085f063b7a8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:05:59 GMT
ADD file:423828ecd1a5225b4d393c372890ff1e90a17fcbe15befc06b94a71fa843ff99 in / 
# Thu, 22 Jul 2021 02:06:01 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:06:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d0aea515a0eca88bed4155cf5a5ed0cd354b107f7892a3eb1d09d93bda2a2722`  
		Last Modified: Thu, 22 Jul 2021 02:19:22 GMT  
		Size: 45.9 MB (45917242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bfac2ff92d5ae0573f40cbd227b707227d5ff11fca1b5959ac52d92bcc6ba5`  
		Last Modified: Thu, 22 Jul 2021 02:19:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4edc325a8e0f60086ccc3a92bd7e35b05f2457db47cad8de170fa482b24f0bb0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49222343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c3b50bfd1e6d9a6cf9c953d80b08dbae9fa8afeb44d888d30133d6ad9390c5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:04 GMT
ADD file:bc14393dda57541decd3b535650114a20bb2a646adbfcc2b0649fa41278df4e3 in / 
# Thu, 22 Jul 2021 00:41:04 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:41:10 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4aaffccfb3fc5a569f4c5f47d342577efb15739f35f37f3f3f8562b6971db6ad`  
		Last Modified: Thu, 22 Jul 2021 00:47:35 GMT  
		Size: 49.2 MB (49222119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d93e557a67ca58ca2f60eafa96251f128c986a181ba60f421e0bdd209a03beb`  
		Last Modified: Thu, 22 Jul 2021 00:47:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:2e2b742d36fa11427654404cd93a18008abdd5410d507aa2f630dbad83c635f1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51206987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c366a11be44194c0f27edb8a9ebbb2eefc76b689bfe400ee3fddba3b10142142`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:00 GMT
ADD file:8e55b0e3d115c6366237668311c2356a0ba2a47cd0d7fb73723647f4087298e5 in / 
# Thu, 22 Jul 2021 00:41:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:41:06 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5383c85c156c662eb185840d8e39387ae2770c823e47ce2f3f5e6a9962980823`  
		Last Modified: Thu, 22 Jul 2021 00:48:34 GMT  
		Size: 51.2 MB (51206762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfb5f46bd54546045a11e1e581c2a069a8e7b004f7daa150c03a4429172e215`  
		Last Modified: Thu, 22 Jul 2021 00:48:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:cac296e1e5238a997b9599134e14a2ff1dc28b9e88ee82c6e2fc64594ab6e005
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49080797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db17e789a7f86c39e64f36299077abcc83ae42eaf1465e6b3cfa35a189c8104f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:10:54 GMT
ADD file:1e3050e1af9a5c4a22c7d5c111c95dad355ebf33a63e9b79e24209dafe47e323 in / 
# Thu, 22 Jul 2021 00:10:55 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:11:01 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:65e8edc868bfb4722a68ca91287781b4a8649557b81323c4d9bc02fc0dbfa9d4`  
		Last Modified: Thu, 22 Jul 2021 00:18:11 GMT  
		Size: 49.1 MB (49080573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9d8dd950004a14797c95ef4fe70aaf88cdfd2e42afa050768469d55abc16b`  
		Last Modified: Thu, 22 Jul 2021 00:18:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:100b3e9120d22b878d6d53cbae425876a75d2b086a0ed416bb89fdafc8936e27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54182650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b82e5ec4a201452546151568c75bca681f6ab0d34911ba905e4c6ecbb496d9c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:20:10 GMT
ADD file:a10e852603be4a8537006299bc6490a15181efa7c6bdc8c2278dd664c5b4bf38 in / 
# Thu, 22 Jul 2021 00:20:18 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:20:39 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:faee74d5cbeba300698783b9582af087f649d5b17d4adeafea63f7482a1d2b2b`  
		Last Modified: Thu, 22 Jul 2021 00:29:01 GMT  
		Size: 54.2 MB (54182424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39d82f7fb457f0d1a67dfc1d8353ddf18164f873f5453650221bf15659f8bff`  
		Last Modified: Thu, 22 Jul 2021 00:29:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:3a0d66e9ab7f34385a8fa9d152a70b85c39245616c52d5921c7d0bcb79a55753
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49004003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c96d592d354e1ac45ec24a7e63778ca77ed4936c1d1e20e3d7a37c69ade7e57`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:43:30 GMT
ADD file:14e3a940c66c70d04bce67d35ac71518affc63c067b19c183538f60b13b0241b in / 
# Thu, 22 Jul 2021 00:43:34 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:43:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4c4c2e7cab9fd5c5a81bd5f2aec15170c676991a90a7f306054ee7c88891352a`  
		Last Modified: Thu, 22 Jul 2021 00:49:00 GMT  
		Size: 49.0 MB (49003779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0388fcbb49c0b56b9a63b7c68e2c598d4124bad01d68c211cf5140160ca53234`  
		Last Modified: Thu, 22 Jul 2021 00:49:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
