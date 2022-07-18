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
-	[`amazonlinux:2022.0.20220628.8`](#amazonlinux20220202206288)
-	[`amazonlinux:2022.0.20220628.8-with-sources`](#amazonlinux20220202206288-with-sources)
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
$ docker pull amazonlinux@sha256:b82f6b670e058ad5fa0a70a2c341399ecaca74cee46b00e27ab34499d0828301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:88c1cec4af4ad05a95697520ce99fa46b00f399568083e08698c9365a498bd40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68790038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae3f3ebc68ce62c498ec6a17cc7962f8009902bcaff28d19439d76ef4592d1f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Jun 2022 22:19:29 GMT
ADD file:3cc0d880def73a3d39f2ec8da9923e1d9311fbb286f57f0354ee67812655e9cc in / 
# Thu, 30 Jun 2022 22:19:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:67cf6ceed7a460575d469086894c81433cddb3fe8a258514d0619c8d7a1f1ec6`  
		Last Modified: Sat, 25 Jun 2022 04:14:50 GMT  
		Size: 68.8 MB (68790038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:457190efb2971739b0715d79019ae1b78d104f228ed9f486d6b57cc22b9c40dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67477196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca20c6939ae64762f9418ebacb840128f7ce539d426b735806ef68fd61051981`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 17:39:42 GMT
ADD file:00537eb2d5579c8983266ab7fe474cd529f7015e22ac65dd87541e46b0d04efc in / 
# Mon, 18 Jul 2022 17:39:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a409f18bc031ea68bf438f175b290c5730af908a1f5eacd4d3ed628376ef728b`  
		Last Modified: Mon, 18 Jul 2022 17:40:51 GMT  
		Size: 67.5 MB (67477196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:344ff4b1f4393a196c004008cbf7a6382a0b1350926be200d8aa2af2f1312d00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:674bb59511e82c8a1c2d258fdcfc7a53a179669a9ebc795d480cb9a4bf8b6168
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.0 MB (483963823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea24a33c3438f88cbb312990d340600fcc8d3cc9e09e8a6b1f4f4bfc3bc4a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Jun 2022 22:19:29 GMT
ADD file:3cc0d880def73a3d39f2ec8da9923e1d9311fbb286f57f0354ee67812655e9cc in / 
# Thu, 30 Jun 2022 22:19:30 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 22:19:52 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-ed69c9a13dd98aac57da3e991b6dba1e11b4436b0fb28daca9344392622a25bc.tar.gz"     && echo "a952c3af116216571c43cf213c443310c15a0687256336904b5d98f9d7fe393d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:67cf6ceed7a460575d469086894c81433cddb3fe8a258514d0619c8d7a1f1ec6`  
		Last Modified: Sat, 25 Jun 2022 04:14:50 GMT  
		Size: 68.8 MB (68790038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92b5f39cc6d3846d4fd81cba740c98bef113e094ecb3de3798b0f03411997e2`  
		Last Modified: Thu, 30 Jun 2022 22:21:01 GMT  
		Size: 415.2 MB (415173785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:241d31e6ceef519880bcdd19a203c569b2ca35e95483660b6dcd8aa38e12b4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.0 MB (481983659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:748231095de7ce3c656cfc5664207291ea55b54726e4d61a7baf421e018b8f0a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 17:39:42 GMT
ADD file:00537eb2d5579c8983266ab7fe474cd529f7015e22ac65dd87541e46b0d04efc in / 
# Mon, 18 Jul 2022 17:39:44 GMT
CMD ["/bin/bash"]
# Mon, 18 Jul 2022 17:40:06 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6ad9d68b91be6ac7e867c110accb52ae5eea9db45924a4ca3d4d32cde09c2f0a.tar.gz"     && echo "70a0d5140609568de4135eb7074409d868e13d33b0fceeca6e06ba401cf47f70  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a409f18bc031ea68bf438f175b290c5730af908a1f5eacd4d3ed628376ef728b`  
		Last Modified: Mon, 18 Jul 2022 17:40:51 GMT  
		Size: 67.5 MB (67477196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ebb50bc68ff064c69dba9f8a55ddeace2ba2b508f32cf6727a987d16d4c479`  
		Last Modified: Mon, 18 Jul 2022 17:41:26 GMT  
		Size: 414.5 MB (414506463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220628.8`

```console
$ docker pull amazonlinux@sha256:0b2cf53597f86f39225736f2cdbeeb2b5d3ed7c60203a48921a527d80eb6a274
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220628.8` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:457190efb2971739b0715d79019ae1b78d104f228ed9f486d6b57cc22b9c40dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67477196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca20c6939ae64762f9418ebacb840128f7ce539d426b735806ef68fd61051981`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 17:39:42 GMT
ADD file:00537eb2d5579c8983266ab7fe474cd529f7015e22ac65dd87541e46b0d04efc in / 
# Mon, 18 Jul 2022 17:39:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a409f18bc031ea68bf438f175b290c5730af908a1f5eacd4d3ed628376ef728b`  
		Last Modified: Mon, 18 Jul 2022 17:40:51 GMT  
		Size: 67.5 MB (67477196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220628.8-with-sources`

```console
$ docker pull amazonlinux@sha256:48e7d872916ee692d745af89ec3e245177d30ffa8de0ce1cfc83161a06d0f836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220628.8-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:241d31e6ceef519880bcdd19a203c569b2ca35e95483660b6dcd8aa38e12b4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.0 MB (481983659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:748231095de7ce3c656cfc5664207291ea55b54726e4d61a7baf421e018b8f0a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 17:39:42 GMT
ADD file:00537eb2d5579c8983266ab7fe474cd529f7015e22ac65dd87541e46b0d04efc in / 
# Mon, 18 Jul 2022 17:39:44 GMT
CMD ["/bin/bash"]
# Mon, 18 Jul 2022 17:40:06 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6ad9d68b91be6ac7e867c110accb52ae5eea9db45924a4ca3d4d32cde09c2f0a.tar.gz"     && echo "70a0d5140609568de4135eb7074409d868e13d33b0fceeca6e06ba401cf47f70  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a409f18bc031ea68bf438f175b290c5730af908a1f5eacd4d3ed628376ef728b`  
		Last Modified: Mon, 18 Jul 2022 17:40:51 GMT  
		Size: 67.5 MB (67477196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ebb50bc68ff064c69dba9f8a55ddeace2ba2b508f32cf6727a987d16d4c479`  
		Last Modified: Mon, 18 Jul 2022 17:41:26 GMT  
		Size: 414.5 MB (414506463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:b82f6b670e058ad5fa0a70a2c341399ecaca74cee46b00e27ab34499d0828301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:88c1cec4af4ad05a95697520ce99fa46b00f399568083e08698c9365a498bd40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68790038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae3f3ebc68ce62c498ec6a17cc7962f8009902bcaff28d19439d76ef4592d1f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Jun 2022 22:19:29 GMT
ADD file:3cc0d880def73a3d39f2ec8da9923e1d9311fbb286f57f0354ee67812655e9cc in / 
# Thu, 30 Jun 2022 22:19:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:67cf6ceed7a460575d469086894c81433cddb3fe8a258514d0619c8d7a1f1ec6`  
		Last Modified: Sat, 25 Jun 2022 04:14:50 GMT  
		Size: 68.8 MB (68790038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:457190efb2971739b0715d79019ae1b78d104f228ed9f486d6b57cc22b9c40dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67477196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca20c6939ae64762f9418ebacb840128f7ce539d426b735806ef68fd61051981`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 17:39:42 GMT
ADD file:00537eb2d5579c8983266ab7fe474cd529f7015e22ac65dd87541e46b0d04efc in / 
# Mon, 18 Jul 2022 17:39:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a409f18bc031ea68bf438f175b290c5730af908a1f5eacd4d3ed628376ef728b`  
		Last Modified: Mon, 18 Jul 2022 17:40:51 GMT  
		Size: 67.5 MB (67477196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:344ff4b1f4393a196c004008cbf7a6382a0b1350926be200d8aa2af2f1312d00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:674bb59511e82c8a1c2d258fdcfc7a53a179669a9ebc795d480cb9a4bf8b6168
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.0 MB (483963823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea24a33c3438f88cbb312990d340600fcc8d3cc9e09e8a6b1f4f4bfc3bc4a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Jun 2022 22:19:29 GMT
ADD file:3cc0d880def73a3d39f2ec8da9923e1d9311fbb286f57f0354ee67812655e9cc in / 
# Thu, 30 Jun 2022 22:19:30 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 22:19:52 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-ed69c9a13dd98aac57da3e991b6dba1e11b4436b0fb28daca9344392622a25bc.tar.gz"     && echo "a952c3af116216571c43cf213c443310c15a0687256336904b5d98f9d7fe393d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:67cf6ceed7a460575d469086894c81433cddb3fe8a258514d0619c8d7a1f1ec6`  
		Last Modified: Sat, 25 Jun 2022 04:14:50 GMT  
		Size: 68.8 MB (68790038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92b5f39cc6d3846d4fd81cba740c98bef113e094ecb3de3798b0f03411997e2`  
		Last Modified: Thu, 30 Jun 2022 22:21:01 GMT  
		Size: 415.2 MB (415173785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:241d31e6ceef519880bcdd19a203c569b2ca35e95483660b6dcd8aa38e12b4d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.0 MB (481983659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:748231095de7ce3c656cfc5664207291ea55b54726e4d61a7baf421e018b8f0a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 17:39:42 GMT
ADD file:00537eb2d5579c8983266ab7fe474cd529f7015e22ac65dd87541e46b0d04efc in / 
# Mon, 18 Jul 2022 17:39:44 GMT
CMD ["/bin/bash"]
# Mon, 18 Jul 2022 17:40:06 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6ad9d68b91be6ac7e867c110accb52ae5eea9db45924a4ca3d4d32cde09c2f0a.tar.gz"     && echo "70a0d5140609568de4135eb7074409d868e13d33b0fceeca6e06ba401cf47f70  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a409f18bc031ea68bf438f175b290c5730af908a1f5eacd4d3ed628376ef728b`  
		Last Modified: Mon, 18 Jul 2022 17:40:51 GMT  
		Size: 67.5 MB (67477196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ebb50bc68ff064c69dba9f8a55ddeace2ba2b508f32cf6727a987d16d4c479`  
		Last Modified: Mon, 18 Jul 2022 17:41:26 GMT  
		Size: 414.5 MB (414506463 bytes)  
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
