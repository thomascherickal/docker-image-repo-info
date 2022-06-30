<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20220606.1`](#amazonlinux20202206061)
-	[`amazonlinux:2.0.20220606.1-with-sources`](#amazonlinux20202206061-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220609.0`](#amazonlinux2018030202206090)
-	[`amazonlinux:2018.03.0.20220609.0-with-sources`](#amazonlinux2018030202206090-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220531.0`](#amazonlinux20220202205310)
-	[`amazonlinux:2022.0.20220531.0-with-sources`](#amazonlinux20220202205310-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:1e9a09649c7babb110a1b67e9a047b638d1c05e1eea0a0d8660ecc183941a653
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:23ff831a5a7a8b479cc3efd50de0fe5d1a49323b05c7fb2eb398f85bc053eeff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62360448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d822393d3edc7f2f6868c4196ff99e2d3268169a27813835322218eb150daa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 22 Jun 2022 20:20:01 GMT
ADD file:68d3b6d64ee94ebc64fddc466c72f2cff90752cfc07fca23fb4c3eb71e638c0a in / 
# Wed, 22 Jun 2022 20:20:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:856ac18c220706a77a37aff7d92d6c50f57993cea544e14d24650d02a154d89e`  
		Last Modified: Wed, 22 Jun 2022 20:21:12 GMT  
		Size: 62.4 MB (62360448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:1ebc0a4c29cb5a9e4d4894526aa2bc85e9974bd40dbf4d34c1093456556424f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9b74fae4083b3ed095f3ae91b6272f3cedbe3bbb71e4f367563ea21d2bbe5c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515043309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bea2ab30f386fa0269d2414b6c2045299fdfbaec499f6e68966d83a99dfe86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 22 Jun 2022 20:20:01 GMT
ADD file:68d3b6d64ee94ebc64fddc466c72f2cff90752cfc07fca23fb4c3eb71e638c0a in / 
# Wed, 22 Jun 2022 20:20:01 GMT
CMD ["/bin/bash"]
# Wed, 22 Jun 2022 20:20:31 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6d9b73cc5134d5a2e933993f9523e43d4aeb09053e5eb630c478f0a356799ab0.tar.gz"     && echo "8dc0ae49727374fe369b02505859705e731aaf44ed8946fb09fe58d8f30385f7  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:856ac18c220706a77a37aff7d92d6c50f57993cea544e14d24650d02a154d89e`  
		Last Modified: Wed, 22 Jun 2022 20:21:12 GMT  
		Size: 62.4 MB (62360448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e9917d087ab17e0dde2d0d24abee9eb9ccd04918a09e6127feaedb1feeb64`  
		Last Modified: Wed, 22 Jun 2022 20:21:41 GMT  
		Size: 452.7 MB (452682861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:3f9411b3b7a1d113d0900ab73a6640a4296441fe10a438b1a84a78295f5ca7a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c9ce7208912b7897c9a4cb273f20bbfd54fd745d1dd64f5e625fff6778469e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62294977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0e8aec8ddc1c632de57d0b0f2dc7779d823a5b52a8444869bfda0a6a26331b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:06a218d9e2f63e912ffc51c7052c6e632e53dfcf8661f96b4028d7db08f931a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63918642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60535d6b0ffab1b528deb0e35bf28f7f8768fc2ed0cda7f5862e047855c9d0b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:dfa7380ea0a52bd33be4c1eb397875d8f0ae4266d78876bf7370c5a82b4899c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:50ef3e2e55421c716cf57afc28942eff9e67a5b5a9ea1410ce3c92c0f39953d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.0 MB (486032841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958ec2f24245a7af21fdf7ae9018d22e865f3b4415c53eae3a9777a667360e30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
# Tue, 21 Jun 2022 23:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-800a7e3918924b4aaf6f75787edd91de54d919ce798c4adbd8190b5dd187eef0.tar.gz"     && echo "ac78714ecd2ea0972b6b72ae2e7ac4b38e0a2d5f5e4751082abe2f4ceee1033d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f238a85b77bd523c86c594598f8dc108f464737b469c8818a79cc26aeae299e8`  
		Last Modified: Tue, 21 Jun 2022 23:21:14 GMT  
		Size: 423.7 MB (423737864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7b886253583362ee6ebe7f69510a2738cc55ea0a9c1ae8c327e82877b3e88f70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.7 MB (487656467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5cbb8d5c004c62b734c7e854b889852efefd7ffd9133d286802fb5277006779`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Tue, 21 Jun 2022 23:39:54 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-800a7e3918924b4aaf6f75787edd91de54d919ce798c4adbd8190b5dd187eef0.tar.gz"     && echo "ac78714ecd2ea0972b6b72ae2e7ac4b38e0a2d5f5e4751082abe2f4ceee1033d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488a72b37e827ac074cd544586f45070542b3658a4623a5da30a6d844f1d79e9`  
		Last Modified: Tue, 21 Jun 2022 23:41:24 GMT  
		Size: 423.7 MB (423737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220606.1`

```console
$ docker pull amazonlinux@sha256:3f9411b3b7a1d113d0900ab73a6640a4296441fe10a438b1a84a78295f5ca7a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220606.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c9ce7208912b7897c9a4cb273f20bbfd54fd745d1dd64f5e625fff6778469e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62294977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0e8aec8ddc1c632de57d0b0f2dc7779d823a5b52a8444869bfda0a6a26331b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220606.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:06a218d9e2f63e912ffc51c7052c6e632e53dfcf8661f96b4028d7db08f931a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63918642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60535d6b0ffab1b528deb0e35bf28f7f8768fc2ed0cda7f5862e047855c9d0b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220606.1-with-sources`

```console
$ docker pull amazonlinux@sha256:dfa7380ea0a52bd33be4c1eb397875d8f0ae4266d78876bf7370c5a82b4899c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220606.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:50ef3e2e55421c716cf57afc28942eff9e67a5b5a9ea1410ce3c92c0f39953d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.0 MB (486032841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958ec2f24245a7af21fdf7ae9018d22e865f3b4415c53eae3a9777a667360e30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
# Tue, 21 Jun 2022 23:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-800a7e3918924b4aaf6f75787edd91de54d919ce798c4adbd8190b5dd187eef0.tar.gz"     && echo "ac78714ecd2ea0972b6b72ae2e7ac4b38e0a2d5f5e4751082abe2f4ceee1033d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f238a85b77bd523c86c594598f8dc108f464737b469c8818a79cc26aeae299e8`  
		Last Modified: Tue, 21 Jun 2022 23:21:14 GMT  
		Size: 423.7 MB (423737864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220606.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7b886253583362ee6ebe7f69510a2738cc55ea0a9c1ae8c327e82877b3e88f70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.7 MB (487656467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5cbb8d5c004c62b734c7e854b889852efefd7ffd9133d286802fb5277006779`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Tue, 21 Jun 2022 23:39:54 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-800a7e3918924b4aaf6f75787edd91de54d919ce798c4adbd8190b5dd187eef0.tar.gz"     && echo "ac78714ecd2ea0972b6b72ae2e7ac4b38e0a2d5f5e4751082abe2f4ceee1033d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488a72b37e827ac074cd544586f45070542b3658a4623a5da30a6d844f1d79e9`  
		Last Modified: Tue, 21 Jun 2022 23:41:24 GMT  
		Size: 423.7 MB (423737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:1e9a09649c7babb110a1b67e9a047b638d1c05e1eea0a0d8660ecc183941a653
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:23ff831a5a7a8b479cc3efd50de0fe5d1a49323b05c7fb2eb398f85bc053eeff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62360448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d822393d3edc7f2f6868c4196ff99e2d3268169a27813835322218eb150daa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 22 Jun 2022 20:20:01 GMT
ADD file:68d3b6d64ee94ebc64fddc466c72f2cff90752cfc07fca23fb4c3eb71e638c0a in / 
# Wed, 22 Jun 2022 20:20:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:856ac18c220706a77a37aff7d92d6c50f57993cea544e14d24650d02a154d89e`  
		Last Modified: Wed, 22 Jun 2022 20:21:12 GMT  
		Size: 62.4 MB (62360448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:1ebc0a4c29cb5a9e4d4894526aa2bc85e9974bd40dbf4d34c1093456556424f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9b74fae4083b3ed095f3ae91b6272f3cedbe3bbb71e4f367563ea21d2bbe5c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515043309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bea2ab30f386fa0269d2414b6c2045299fdfbaec499f6e68966d83a99dfe86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 22 Jun 2022 20:20:01 GMT
ADD file:68d3b6d64ee94ebc64fddc466c72f2cff90752cfc07fca23fb4c3eb71e638c0a in / 
# Wed, 22 Jun 2022 20:20:01 GMT
CMD ["/bin/bash"]
# Wed, 22 Jun 2022 20:20:31 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6d9b73cc5134d5a2e933993f9523e43d4aeb09053e5eb630c478f0a356799ab0.tar.gz"     && echo "8dc0ae49727374fe369b02505859705e731aaf44ed8946fb09fe58d8f30385f7  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:856ac18c220706a77a37aff7d92d6c50f57993cea544e14d24650d02a154d89e`  
		Last Modified: Wed, 22 Jun 2022 20:21:12 GMT  
		Size: 62.4 MB (62360448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e9917d087ab17e0dde2d0d24abee9eb9ccd04918a09e6127feaedb1feeb64`  
		Last Modified: Wed, 22 Jun 2022 20:21:41 GMT  
		Size: 452.7 MB (452682861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220609.0`

```console
$ docker pull amazonlinux@sha256:1e9a09649c7babb110a1b67e9a047b638d1c05e1eea0a0d8660ecc183941a653
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220609.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:23ff831a5a7a8b479cc3efd50de0fe5d1a49323b05c7fb2eb398f85bc053eeff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62360448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d822393d3edc7f2f6868c4196ff99e2d3268169a27813835322218eb150daa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 22 Jun 2022 20:20:01 GMT
ADD file:68d3b6d64ee94ebc64fddc466c72f2cff90752cfc07fca23fb4c3eb71e638c0a in / 
# Wed, 22 Jun 2022 20:20:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:856ac18c220706a77a37aff7d92d6c50f57993cea544e14d24650d02a154d89e`  
		Last Modified: Wed, 22 Jun 2022 20:21:12 GMT  
		Size: 62.4 MB (62360448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220609.0-with-sources`

```console
$ docker pull amazonlinux@sha256:1ebc0a4c29cb5a9e4d4894526aa2bc85e9974bd40dbf4d34c1093456556424f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220609.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9b74fae4083b3ed095f3ae91b6272f3cedbe3bbb71e4f367563ea21d2bbe5c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515043309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bea2ab30f386fa0269d2414b6c2045299fdfbaec499f6e68966d83a99dfe86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 22 Jun 2022 20:20:01 GMT
ADD file:68d3b6d64ee94ebc64fddc466c72f2cff90752cfc07fca23fb4c3eb71e638c0a in / 
# Wed, 22 Jun 2022 20:20:01 GMT
CMD ["/bin/bash"]
# Wed, 22 Jun 2022 20:20:31 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6d9b73cc5134d5a2e933993f9523e43d4aeb09053e5eb630c478f0a356799ab0.tar.gz"     && echo "8dc0ae49727374fe369b02505859705e731aaf44ed8946fb09fe58d8f30385f7  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:856ac18c220706a77a37aff7d92d6c50f57993cea544e14d24650d02a154d89e`  
		Last Modified: Wed, 22 Jun 2022 20:21:12 GMT  
		Size: 62.4 MB (62360448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e9917d087ab17e0dde2d0d24abee9eb9ccd04918a09e6127feaedb1feeb64`  
		Last Modified: Wed, 22 Jun 2022 20:21:41 GMT  
		Size: 452.7 MB (452682861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:3b1eddcdaaf8d664e960b9d48c77c29ee81f108e54673e4015f924993ea81cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:8453a47334b50bd11a6dc8a9ff7c3e40a4ba284f0dc68c5e0edf328b11fe372f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70559972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dbdf168f78243e4eec0ca6653835b7c0d5723635f3956c67c801241670d5d17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6254b7a9191c78cc08dfbdf1becd92b54a76d7976043bcd31ab104982d65b736
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69117442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bea8bae0c8c1a8e3676cee260156f268461e8787f92d1a62e7ccccc1f4bca19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:95e0415cbddc9a78c7c3d739fb7f7dba165b3608489c651e106b16f7ce9fb442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:302cafedc0bb193cb86bbf729250cfe5198abb36814f5073704a5d31fb76408a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489309531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b46dbb32e5b71640810f230fa6749b7c2d6b43be596cd2052cbfb85bec4c5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:39 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a4b54850ae445fac5d810015c4dce9a59828591287cf034e8d8687a5f42db1`  
		Last Modified: Thu, 12 May 2022 22:55:34 GMT  
		Size: 418.7 MB (418749559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:db26696e2371b0e24bc72edf8c118bd9cb18821dfe4f2343495d33eb93aaf2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.9 MB (487866967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7afbb6532b42550d7ce56e9d45b1a30eddbbdf33eef198e4ba4b1123cf9ae38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:03:35 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f37a59badfcabe5a4ef65d9e6f67b552297ca000f896c8a7f5bffc17447a49`  
		Last Modified: Thu, 12 May 2022 22:05:01 GMT  
		Size: 418.7 MB (418749525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220531.0`

**does not exist** (yet?)

## `amazonlinux:2022.0.20220531.0-with-sources`

**does not exist** (yet?)

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:3b1eddcdaaf8d664e960b9d48c77c29ee81f108e54673e4015f924993ea81cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:8453a47334b50bd11a6dc8a9ff7c3e40a4ba284f0dc68c5e0edf328b11fe372f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70559972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dbdf168f78243e4eec0ca6653835b7c0d5723635f3956c67c801241670d5d17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6254b7a9191c78cc08dfbdf1becd92b54a76d7976043bcd31ab104982d65b736
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69117442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bea8bae0c8c1a8e3676cee260156f268461e8787f92d1a62e7ccccc1f4bca19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:95e0415cbddc9a78c7c3d739fb7f7dba165b3608489c651e106b16f7ce9fb442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:302cafedc0bb193cb86bbf729250cfe5198abb36814f5073704a5d31fb76408a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489309531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b46dbb32e5b71640810f230fa6749b7c2d6b43be596cd2052cbfb85bec4c5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:39 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a4b54850ae445fac5d810015c4dce9a59828591287cf034e8d8687a5f42db1`  
		Last Modified: Thu, 12 May 2022 22:55:34 GMT  
		Size: 418.7 MB (418749559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:db26696e2371b0e24bc72edf8c118bd9cb18821dfe4f2343495d33eb93aaf2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.9 MB (487866967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7afbb6532b42550d7ce56e9d45b1a30eddbbdf33eef198e4ba4b1123cf9ae38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:03:35 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f37a59badfcabe5a4ef65d9e6f67b552297ca000f896c8a7f5bffc17447a49`  
		Last Modified: Thu, 12 May 2022 22:05:01 GMT  
		Size: 418.7 MB (418749525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:3f9411b3b7a1d113d0900ab73a6640a4296441fe10a438b1a84a78295f5ca7a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c9ce7208912b7897c9a4cb273f20bbfd54fd745d1dd64f5e625fff6778469e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62294977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0e8aec8ddc1c632de57d0b0f2dc7779d823a5b52a8444869bfda0a6a26331b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:06a218d9e2f63e912ffc51c7052c6e632e53dfcf8661f96b4028d7db08f931a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63918642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60535d6b0ffab1b528deb0e35bf28f7f8768fc2ed0cda7f5862e047855c9d0b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:dfa7380ea0a52bd33be4c1eb397875d8f0ae4266d78876bf7370c5a82b4899c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:50ef3e2e55421c716cf57afc28942eff9e67a5b5a9ea1410ce3c92c0f39953d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.0 MB (486032841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958ec2f24245a7af21fdf7ae9018d22e865f3b4415c53eae3a9777a667360e30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
# Tue, 21 Jun 2022 23:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-800a7e3918924b4aaf6f75787edd91de54d919ce798c4adbd8190b5dd187eef0.tar.gz"     && echo "ac78714ecd2ea0972b6b72ae2e7ac4b38e0a2d5f5e4751082abe2f4ceee1033d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f238a85b77bd523c86c594598f8dc108f464737b469c8818a79cc26aeae299e8`  
		Last Modified: Tue, 21 Jun 2022 23:21:14 GMT  
		Size: 423.7 MB (423737864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7b886253583362ee6ebe7f69510a2738cc55ea0a9c1ae8c327e82877b3e88f70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.7 MB (487656467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5cbb8d5c004c62b734c7e854b889852efefd7ffd9133d286802fb5277006779`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Tue, 21 Jun 2022 23:39:54 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-800a7e3918924b4aaf6f75787edd91de54d919ce798c4adbd8190b5dd187eef0.tar.gz"     && echo "ac78714ecd2ea0972b6b72ae2e7ac4b38e0a2d5f5e4751082abe2f4ceee1033d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488a72b37e827ac074cd544586f45070542b3658a4623a5da30a6d844f1d79e9`  
		Last Modified: Tue, 21 Jun 2022 23:41:24 GMT  
		Size: 423.7 MB (423737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
