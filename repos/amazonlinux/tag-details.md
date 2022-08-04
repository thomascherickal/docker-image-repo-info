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
-	[`amazonlinux:2018.03.0.20220705.1`](#amazonlinux2018030202207051)
-	[`amazonlinux:2018.03.0.20220705.1-with-sources`](#amazonlinux2018030202207051-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220728.1`](#amazonlinux20220202207281)
-	[`amazonlinux:2022.0.20220728.1-with-sources`](#amazonlinux20220202207281-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:4c2c7b34d4195b4de02111d15ff93b0b6df45f5514a4d13ef6fd6014fa02c091
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7469889f01ba05936a481dec30931832c0887783ab94b82c557029d521cb2773
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62349761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5ab74eaa7e03d0ade2d3efb77c8adfb3f9dfd95002a9e098afd17f3c2e826d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Aug 2022 00:19:44 GMT
ADD file:578d048adbda4319c9c7a4cc58359e1b2120c1fea0bdd7af885085f085b76543 in / 
# Thu, 04 Aug 2022 00:19:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0c99b462d7b9e003ee491b5822729d97c1a950b380b4ed0d31dd841909eaaa47`  
		Last Modified: Thu, 04 Aug 2022 00:20:52 GMT  
		Size: 62.3 MB (62349761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:4185f05daac0e029ed74065c968aa3550738e71f28f865afb203e48443d8f25d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:d587f87e29ec3c73030808824cd64ffc259edf7ec172feafe2eeaab6452dfb79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515034837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1862d4c5d4530382c100d0ad62b44402dd8056ca13a22de7b6c7b0928fc06538`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Aug 2022 00:19:44 GMT
ADD file:578d048adbda4319c9c7a4cc58359e1b2120c1fea0bdd7af885085f085b76543 in / 
# Thu, 04 Aug 2022 00:19:45 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:20:11 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-88cdcaaae92c13e9b16f4e24733dac64044525869a4d99c16f84d49e67daaf62.tar.gz"     && echo "4f388bc0087173f93599d0e9c5b6548cfea6212e7e88c1955793515a6efdae5b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0c99b462d7b9e003ee491b5822729d97c1a950b380b4ed0d31dd841909eaaa47`  
		Last Modified: Thu, 04 Aug 2022 00:20:52 GMT  
		Size: 62.3 MB (62349761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566b981add5da336c6f5f83b0f5e18f5360adace1960c3834dde438b258a012a`  
		Last Modified: Thu, 04 Aug 2022 00:21:21 GMT  
		Size: 452.7 MB (452685076 bytes)  
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
$ docker pull amazonlinux@sha256:4c2c7b34d4195b4de02111d15ff93b0b6df45f5514a4d13ef6fd6014fa02c091
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7469889f01ba05936a481dec30931832c0887783ab94b82c557029d521cb2773
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62349761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5ab74eaa7e03d0ade2d3efb77c8adfb3f9dfd95002a9e098afd17f3c2e826d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Aug 2022 00:19:44 GMT
ADD file:578d048adbda4319c9c7a4cc58359e1b2120c1fea0bdd7af885085f085b76543 in / 
# Thu, 04 Aug 2022 00:19:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0c99b462d7b9e003ee491b5822729d97c1a950b380b4ed0d31dd841909eaaa47`  
		Last Modified: Thu, 04 Aug 2022 00:20:52 GMT  
		Size: 62.3 MB (62349761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:4185f05daac0e029ed74065c968aa3550738e71f28f865afb203e48443d8f25d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:d587f87e29ec3c73030808824cd64ffc259edf7ec172feafe2eeaab6452dfb79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515034837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1862d4c5d4530382c100d0ad62b44402dd8056ca13a22de7b6c7b0928fc06538`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Aug 2022 00:19:44 GMT
ADD file:578d048adbda4319c9c7a4cc58359e1b2120c1fea0bdd7af885085f085b76543 in / 
# Thu, 04 Aug 2022 00:19:45 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:20:11 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-88cdcaaae92c13e9b16f4e24733dac64044525869a4d99c16f84d49e67daaf62.tar.gz"     && echo "4f388bc0087173f93599d0e9c5b6548cfea6212e7e88c1955793515a6efdae5b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0c99b462d7b9e003ee491b5822729d97c1a950b380b4ed0d31dd841909eaaa47`  
		Last Modified: Thu, 04 Aug 2022 00:20:52 GMT  
		Size: 62.3 MB (62349761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566b981add5da336c6f5f83b0f5e18f5360adace1960c3834dde438b258a012a`  
		Last Modified: Thu, 04 Aug 2022 00:21:21 GMT  
		Size: 452.7 MB (452685076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220705.1`

```console
$ docker pull amazonlinux@sha256:4c2c7b34d4195b4de02111d15ff93b0b6df45f5514a4d13ef6fd6014fa02c091
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220705.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7469889f01ba05936a481dec30931832c0887783ab94b82c557029d521cb2773
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62349761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5ab74eaa7e03d0ade2d3efb77c8adfb3f9dfd95002a9e098afd17f3c2e826d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Aug 2022 00:19:44 GMT
ADD file:578d048adbda4319c9c7a4cc58359e1b2120c1fea0bdd7af885085f085b76543 in / 
# Thu, 04 Aug 2022 00:19:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0c99b462d7b9e003ee491b5822729d97c1a950b380b4ed0d31dd841909eaaa47`  
		Last Modified: Thu, 04 Aug 2022 00:20:52 GMT  
		Size: 62.3 MB (62349761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220705.1-with-sources`

```console
$ docker pull amazonlinux@sha256:4185f05daac0e029ed74065c968aa3550738e71f28f865afb203e48443d8f25d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220705.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:d587f87e29ec3c73030808824cd64ffc259edf7ec172feafe2eeaab6452dfb79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515034837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1862d4c5d4530382c100d0ad62b44402dd8056ca13a22de7b6c7b0928fc06538`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 Aug 2022 00:19:44 GMT
ADD file:578d048adbda4319c9c7a4cc58359e1b2120c1fea0bdd7af885085f085b76543 in / 
# Thu, 04 Aug 2022 00:19:45 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:20:11 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-88cdcaaae92c13e9b16f4e24733dac64044525869a4d99c16f84d49e67daaf62.tar.gz"     && echo "4f388bc0087173f93599d0e9c5b6548cfea6212e7e88c1955793515a6efdae5b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0c99b462d7b9e003ee491b5822729d97c1a950b380b4ed0d31dd841909eaaa47`  
		Last Modified: Thu, 04 Aug 2022 00:20:52 GMT  
		Size: 62.3 MB (62349761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566b981add5da336c6f5f83b0f5e18f5360adace1960c3834dde438b258a012a`  
		Last Modified: Thu, 04 Aug 2022 00:21:21 GMT  
		Size: 452.7 MB (452685076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:2e7aa9246021b49f25eb4d608b201c5f0d76729b3b96c066349ada3ec0fa5538
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:24e4e6dcf5a93c43262e779ff9e4379f5b2b8e9227143063b547c9ac1ae34678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57848915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bea335b6ed06cf61fda2da202d5562c5393c317d76da0401817d95cbfcf9e1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 14:21:00 GMT
ADD file:502afb431df03ea274b7deb3fa9e2c69be0542f1512c5267c29c42847380bade in / 
# Wed, 03 Aug 2022 14:21:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e848115352d3c0b00738ee4e38e805b2f90162580e873b68273e2656b321e529`  
		Last Modified: Sat, 30 Jul 2022 04:06:16 GMT  
		Size: 57.8 MB (57848915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:19cc84ca97003c4e5b875be85dafbeb338403d29b71839548f9be31aac02e314
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56641949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57d4ca5ed86ff1a81bfc554b778d473a1f37d0a9fa36dccd554de26c08529b9e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 12:14:13 GMT
ADD file:66d41fa1401574d2e46e90ac16b59303f71c7bf398ddb0922a8d1e901ff01a33 in / 
# Wed, 03 Aug 2022 12:14:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:71f53d65e46f63ed07b6ba9d631c781f35a9e3aa0c59d15d2a6b8cf540ea474c`  
		Last Modified: Wed, 03 Aug 2022 12:15:19 GMT  
		Size: 56.6 MB (56641949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:a62d7d9b2d2ac3b5d2483453bdd31610b7af9786c625420a5a0d9d34982710a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3dcac5d2d2a961b3d1c9ff5cc34db60c67e9ae2c3f8a4852dda9605b0639d805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392581873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1361b455f9fc595247355858a3b469f2f09f4eccc7ccb85232513757010ab694`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 14:21:00 GMT
ADD file:502afb431df03ea274b7deb3fa9e2c69be0542f1512c5267c29c42847380bade in / 
# Wed, 03 Aug 2022 14:21:01 GMT
CMD ["/bin/bash"]
# Wed, 03 Aug 2022 14:21:24 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-957d3ae3a19e9ce71b665e8cd92c84fbdd09ac787fc6fe6e529d2eb7dda57e9b.tar.gz"     && echo "e6514c0ba308c79d2d886e936bb17e7b6c5bc1761cc0264a8bf9c7b97d751f2d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e848115352d3c0b00738ee4e38e805b2f90162580e873b68273e2656b321e529`  
		Last Modified: Sat, 30 Jul 2022 04:06:16 GMT  
		Size: 57.8 MB (57848915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed0097bd17206d415e8d836e5e3407fab794e8cf70c0db883bf2c75bb8ba68`  
		Last Modified: Wed, 03 Aug 2022 14:22:31 GMT  
		Size: 334.7 MB (334732958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:06237ff0de1785329f0428e83d7ee58d1430a5f0e33cbde4edcd9dddcf292d7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391374875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972d3f26f41b671359686ec38bc7ed11c9d2c6014e0da98b70e878a176bc0ae7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 12:14:13 GMT
ADD file:66d41fa1401574d2e46e90ac16b59303f71c7bf398ddb0922a8d1e901ff01a33 in / 
# Wed, 03 Aug 2022 12:14:14 GMT
CMD ["/bin/bash"]
# Wed, 03 Aug 2022 12:14:34 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-957d3ae3a19e9ce71b665e8cd92c84fbdd09ac787fc6fe6e529d2eb7dda57e9b.tar.gz"     && echo "e6514c0ba308c79d2d886e936bb17e7b6c5bc1761cc0264a8bf9c7b97d751f2d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:71f53d65e46f63ed07b6ba9d631c781f35a9e3aa0c59d15d2a6b8cf540ea474c`  
		Last Modified: Wed, 03 Aug 2022 12:15:19 GMT  
		Size: 56.6 MB (56641949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cbc02f83028ec35f5475f7de55ed612be3498de9f4689424fd826a703e17c`  
		Last Modified: Wed, 03 Aug 2022 12:16:01 GMT  
		Size: 334.7 MB (334732926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220728.1`

```console
$ docker pull amazonlinux@sha256:2e7aa9246021b49f25eb4d608b201c5f0d76729b3b96c066349ada3ec0fa5538
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220728.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:24e4e6dcf5a93c43262e779ff9e4379f5b2b8e9227143063b547c9ac1ae34678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57848915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bea335b6ed06cf61fda2da202d5562c5393c317d76da0401817d95cbfcf9e1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 14:21:00 GMT
ADD file:502afb431df03ea274b7deb3fa9e2c69be0542f1512c5267c29c42847380bade in / 
# Wed, 03 Aug 2022 14:21:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e848115352d3c0b00738ee4e38e805b2f90162580e873b68273e2656b321e529`  
		Last Modified: Sat, 30 Jul 2022 04:06:16 GMT  
		Size: 57.8 MB (57848915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220728.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:19cc84ca97003c4e5b875be85dafbeb338403d29b71839548f9be31aac02e314
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56641949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57d4ca5ed86ff1a81bfc554b778d473a1f37d0a9fa36dccd554de26c08529b9e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 12:14:13 GMT
ADD file:66d41fa1401574d2e46e90ac16b59303f71c7bf398ddb0922a8d1e901ff01a33 in / 
# Wed, 03 Aug 2022 12:14:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:71f53d65e46f63ed07b6ba9d631c781f35a9e3aa0c59d15d2a6b8cf540ea474c`  
		Last Modified: Wed, 03 Aug 2022 12:15:19 GMT  
		Size: 56.6 MB (56641949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220728.1-with-sources`

```console
$ docker pull amazonlinux@sha256:a62d7d9b2d2ac3b5d2483453bdd31610b7af9786c625420a5a0d9d34982710a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220728.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3dcac5d2d2a961b3d1c9ff5cc34db60c67e9ae2c3f8a4852dda9605b0639d805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392581873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1361b455f9fc595247355858a3b469f2f09f4eccc7ccb85232513757010ab694`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 14:21:00 GMT
ADD file:502afb431df03ea274b7deb3fa9e2c69be0542f1512c5267c29c42847380bade in / 
# Wed, 03 Aug 2022 14:21:01 GMT
CMD ["/bin/bash"]
# Wed, 03 Aug 2022 14:21:24 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-957d3ae3a19e9ce71b665e8cd92c84fbdd09ac787fc6fe6e529d2eb7dda57e9b.tar.gz"     && echo "e6514c0ba308c79d2d886e936bb17e7b6c5bc1761cc0264a8bf9c7b97d751f2d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e848115352d3c0b00738ee4e38e805b2f90162580e873b68273e2656b321e529`  
		Last Modified: Sat, 30 Jul 2022 04:06:16 GMT  
		Size: 57.8 MB (57848915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed0097bd17206d415e8d836e5e3407fab794e8cf70c0db883bf2c75bb8ba68`  
		Last Modified: Wed, 03 Aug 2022 14:22:31 GMT  
		Size: 334.7 MB (334732958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220728.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:06237ff0de1785329f0428e83d7ee58d1430a5f0e33cbde4edcd9dddcf292d7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391374875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972d3f26f41b671359686ec38bc7ed11c9d2c6014e0da98b70e878a176bc0ae7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 12:14:13 GMT
ADD file:66d41fa1401574d2e46e90ac16b59303f71c7bf398ddb0922a8d1e901ff01a33 in / 
# Wed, 03 Aug 2022 12:14:14 GMT
CMD ["/bin/bash"]
# Wed, 03 Aug 2022 12:14:34 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-957d3ae3a19e9ce71b665e8cd92c84fbdd09ac787fc6fe6e529d2eb7dda57e9b.tar.gz"     && echo "e6514c0ba308c79d2d886e936bb17e7b6c5bc1761cc0264a8bf9c7b97d751f2d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:71f53d65e46f63ed07b6ba9d631c781f35a9e3aa0c59d15d2a6b8cf540ea474c`  
		Last Modified: Wed, 03 Aug 2022 12:15:19 GMT  
		Size: 56.6 MB (56641949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cbc02f83028ec35f5475f7de55ed612be3498de9f4689424fd826a703e17c`  
		Last Modified: Wed, 03 Aug 2022 12:16:01 GMT  
		Size: 334.7 MB (334732926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:2e7aa9246021b49f25eb4d608b201c5f0d76729b3b96c066349ada3ec0fa5538
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:24e4e6dcf5a93c43262e779ff9e4379f5b2b8e9227143063b547c9ac1ae34678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57848915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bea335b6ed06cf61fda2da202d5562c5393c317d76da0401817d95cbfcf9e1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 14:21:00 GMT
ADD file:502afb431df03ea274b7deb3fa9e2c69be0542f1512c5267c29c42847380bade in / 
# Wed, 03 Aug 2022 14:21:01 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e848115352d3c0b00738ee4e38e805b2f90162580e873b68273e2656b321e529`  
		Last Modified: Sat, 30 Jul 2022 04:06:16 GMT  
		Size: 57.8 MB (57848915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:19cc84ca97003c4e5b875be85dafbeb338403d29b71839548f9be31aac02e314
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56641949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57d4ca5ed86ff1a81bfc554b778d473a1f37d0a9fa36dccd554de26c08529b9e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 12:14:13 GMT
ADD file:66d41fa1401574d2e46e90ac16b59303f71c7bf398ddb0922a8d1e901ff01a33 in / 
# Wed, 03 Aug 2022 12:14:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:71f53d65e46f63ed07b6ba9d631c781f35a9e3aa0c59d15d2a6b8cf540ea474c`  
		Last Modified: Wed, 03 Aug 2022 12:15:19 GMT  
		Size: 56.6 MB (56641949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:a62d7d9b2d2ac3b5d2483453bdd31610b7af9786c625420a5a0d9d34982710a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3dcac5d2d2a961b3d1c9ff5cc34db60c67e9ae2c3f8a4852dda9605b0639d805
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392581873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1361b455f9fc595247355858a3b469f2f09f4eccc7ccb85232513757010ab694`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 14:21:00 GMT
ADD file:502afb431df03ea274b7deb3fa9e2c69be0542f1512c5267c29c42847380bade in / 
# Wed, 03 Aug 2022 14:21:01 GMT
CMD ["/bin/bash"]
# Wed, 03 Aug 2022 14:21:24 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-957d3ae3a19e9ce71b665e8cd92c84fbdd09ac787fc6fe6e529d2eb7dda57e9b.tar.gz"     && echo "e6514c0ba308c79d2d886e936bb17e7b6c5bc1761cc0264a8bf9c7b97d751f2d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e848115352d3c0b00738ee4e38e805b2f90162580e873b68273e2656b321e529`  
		Last Modified: Sat, 30 Jul 2022 04:06:16 GMT  
		Size: 57.8 MB (57848915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed0097bd17206d415e8d836e5e3407fab794e8cf70c0db883bf2c75bb8ba68`  
		Last Modified: Wed, 03 Aug 2022 14:22:31 GMT  
		Size: 334.7 MB (334732958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:06237ff0de1785329f0428e83d7ee58d1430a5f0e33cbde4edcd9dddcf292d7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391374875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972d3f26f41b671359686ec38bc7ed11c9d2c6014e0da98b70e878a176bc0ae7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 03 Aug 2022 12:14:13 GMT
ADD file:66d41fa1401574d2e46e90ac16b59303f71c7bf398ddb0922a8d1e901ff01a33 in / 
# Wed, 03 Aug 2022 12:14:14 GMT
CMD ["/bin/bash"]
# Wed, 03 Aug 2022 12:14:34 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-957d3ae3a19e9ce71b665e8cd92c84fbdd09ac787fc6fe6e529d2eb7dda57e9b.tar.gz"     && echo "e6514c0ba308c79d2d886e936bb17e7b6c5bc1761cc0264a8bf9c7b97d751f2d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:71f53d65e46f63ed07b6ba9d631c781f35a9e3aa0c59d15d2a6b8cf540ea474c`  
		Last Modified: Wed, 03 Aug 2022 12:15:19 GMT  
		Size: 56.6 MB (56641949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cbc02f83028ec35f5475f7de55ed612be3498de9f4689424fd826a703e17c`  
		Last Modified: Wed, 03 Aug 2022 12:16:01 GMT  
		Size: 334.7 MB (334732926 bytes)  
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
