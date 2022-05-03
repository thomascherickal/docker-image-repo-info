<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20220426.0`](#amazonlinux20202204260)
-	[`amazonlinux:2.0.20220426.0-with-sources`](#amazonlinux20202204260-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220419.0`](#amazonlinux2018030202204190)
-	[`amazonlinux:2018.03.0.20220419.0-with-sources`](#amazonlinux2018030202204190-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220419.0`](#amazonlinux20220202204190)
-	[`amazonlinux:2022.0.20220419.0-with-sources`](#amazonlinux20220202204190-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:7e25084410d24fa4830e619f5331f018bd6e0ac5b53c47f2518a62d5e92a2cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:070a330b34fa85275ac40541a830d43b30aadc2a773648da9457dd6c003e47bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62368733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719a671add20f6fa0b850e3023e7d6115cdd2061ac571b1ec74f814cc2af8806`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 23 Apr 2022 01:20:58 GMT
ADD file:648f5c0af52d0f60f0c9312ed88484b5c47f37512d1da91cd171bfd6bd3eb693 in / 
# Sat, 23 Apr 2022 01:20:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1651c8ca9fa2a1211ca3981a04760e4249b1ea5248c4650a768844c5bafa933`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 62.4 MB (62368733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:7c3adb037884d64f74753449315d0959969861102acaaa75e701e8e1d61bd2b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7b10e3edb3d85f719b0120d8fc02d6ae777e93b9996718df2caa826338c57a11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515018819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f74812e89dff5d7417f213101574bcafb217529538925d94bd5522e5df5ef86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 23 Apr 2022 01:20:58 GMT
ADD file:648f5c0af52d0f60f0c9312ed88484b5c47f37512d1da91cd171bfd6bd3eb693 in / 
# Sat, 23 Apr 2022 01:20:58 GMT
CMD ["/bin/bash"]
# Sat, 23 Apr 2022 01:21:23 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3218b580f105e26d79916fd58a49937f9ae8cd25196a762d6e47d1d6c891e437.tar.gz"  && echo "c2cc764bbb63b9eaba23de4bd298faf993093ba4d8098eed411753d88dc9cde6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d1651c8ca9fa2a1211ca3981a04760e4249b1ea5248c4650a768844c5bafa933`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 62.4 MB (62368733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0423df311996171a2ece9630104cac5b1ec4f5c5c3024bca6d9ce573f8f00f64`  
		Last Modified: Sat, 23 Apr 2022 01:22:32 GMT  
		Size: 452.7 MB (452650086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:54f592d954725ce989af5ed5fb49e35ab2b1f1d830ee3f1f79b58ed75a631f64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1301cc9f889f21dc45733df9e58034ac1c318202b4b0f0a08d88b3fdc03004de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62265199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365842604a8b06c7c6dcb1ead27ee7297138603dc36dd4a64fe0421100256334`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:19:57 GMT
ADD file:4eb88d9d977dadb40c630d693a07ca066069b30b9751b7a421dfb4ba0b99d862 in / 
# Thu, 21 Apr 2022 22:19:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ac1397dc8419bf1767b60a5cc5849b7130406030581d4542e48965801c303a70`  
		Last Modified: Thu, 21 Apr 2022 22:08:36 GMT  
		Size: 62.3 MB (62265199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2249ff9b9983e5b9983c560645d6378f825827723b4a8c8a30ccb6d8cb661276
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63888157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:583d35ff5db28103719d2359a7e631acc8e85896a9ca9fb45f99fd36511c1aae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:57:49 GMT
ADD file:76e1ee72575f50a75573a46483631e239d3b6afda9fdd53086883bd03db5364b in / 
# Thu, 21 Apr 2022 22:57:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86bcd0b49e3391c117b5e27756fdf585aadc1a7b9054d19af0faa050839a6633`  
		Last Modified: Thu, 21 Apr 2022 22:59:02 GMT  
		Size: 63.9 MB (63888157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:c2f343c1353778866e90fba96b5b6173b255f07d302de7c0703c9c67d1c863f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:67fd44e1ca29a3c41ea875774083e64f218643232b1f5f27dfb1b1e4b6aeebf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485656205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511c70976d4f4738c09199e01633142618f58f7bc2345948fa514aba7741d28e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:19:57 GMT
ADD file:4eb88d9d977dadb40c630d693a07ca066069b30b9751b7a421dfb4ba0b99d862 in / 
# Thu, 21 Apr 2022 22:19:58 GMT
CMD ["/bin/bash"]
# Thu, 21 Apr 2022 22:20:24 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-915f4823664b0d5efa5a9e17372f52c1e32718dcd0045d286495168c62f27bf6.tar.gz"  && echo "ddee5f71296afcb2dc85200f657f30688a3edb91a3e317592c02d9b387c62d5b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ac1397dc8419bf1767b60a5cc5849b7130406030581d4542e48965801c303a70`  
		Last Modified: Thu, 21 Apr 2022 22:08:36 GMT  
		Size: 62.3 MB (62265199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf04fc591da032b75c5a1e2f399e07e93a1b66b3bc75b07fe457ede25a29d9d`  
		Last Modified: Thu, 21 Apr 2022 22:21:31 GMT  
		Size: 423.4 MB (423391006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9ef53f86fd3105e8d6ed9465463739e3c672d0fb995722e7a7a0abf09bd2954b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487279116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a0bc6da757fa79443ed42fd5cf1b1909702466a8a507cfc78ca9f1ea291a09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:57:49 GMT
ADD file:76e1ee72575f50a75573a46483631e239d3b6afda9fdd53086883bd03db5364b in / 
# Thu, 21 Apr 2022 22:57:51 GMT
CMD ["/bin/bash"]
# Thu, 21 Apr 2022 22:58:15 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-915f4823664b0d5efa5a9e17372f52c1e32718dcd0045d286495168c62f27bf6.tar.gz"  && echo "ddee5f71296afcb2dc85200f657f30688a3edb91a3e317592c02d9b387c62d5b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:86bcd0b49e3391c117b5e27756fdf585aadc1a7b9054d19af0faa050839a6633`  
		Last Modified: Thu, 21 Apr 2022 22:59:02 GMT  
		Size: 63.9 MB (63888157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17307b92b5f720ad82dc04ee1d549790061ada9c458c29252ff0e64f85017078`  
		Last Modified: Thu, 21 Apr 2022 22:59:56 GMT  
		Size: 423.4 MB (423390959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220426.0`

**does not exist** (yet?)

## `amazonlinux:2.0.20220426.0-with-sources`

**does not exist** (yet?)

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:7e25084410d24fa4830e619f5331f018bd6e0ac5b53c47f2518a62d5e92a2cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:070a330b34fa85275ac40541a830d43b30aadc2a773648da9457dd6c003e47bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62368733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719a671add20f6fa0b850e3023e7d6115cdd2061ac571b1ec74f814cc2af8806`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 23 Apr 2022 01:20:58 GMT
ADD file:648f5c0af52d0f60f0c9312ed88484b5c47f37512d1da91cd171bfd6bd3eb693 in / 
# Sat, 23 Apr 2022 01:20:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1651c8ca9fa2a1211ca3981a04760e4249b1ea5248c4650a768844c5bafa933`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 62.4 MB (62368733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:7c3adb037884d64f74753449315d0959969861102acaaa75e701e8e1d61bd2b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7b10e3edb3d85f719b0120d8fc02d6ae777e93b9996718df2caa826338c57a11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515018819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f74812e89dff5d7417f213101574bcafb217529538925d94bd5522e5df5ef86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 23 Apr 2022 01:20:58 GMT
ADD file:648f5c0af52d0f60f0c9312ed88484b5c47f37512d1da91cd171bfd6bd3eb693 in / 
# Sat, 23 Apr 2022 01:20:58 GMT
CMD ["/bin/bash"]
# Sat, 23 Apr 2022 01:21:23 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3218b580f105e26d79916fd58a49937f9ae8cd25196a762d6e47d1d6c891e437.tar.gz"  && echo "c2cc764bbb63b9eaba23de4bd298faf993093ba4d8098eed411753d88dc9cde6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d1651c8ca9fa2a1211ca3981a04760e4249b1ea5248c4650a768844c5bafa933`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 62.4 MB (62368733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0423df311996171a2ece9630104cac5b1ec4f5c5c3024bca6d9ce573f8f00f64`  
		Last Modified: Sat, 23 Apr 2022 01:22:32 GMT  
		Size: 452.7 MB (452650086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220419.0`

```console
$ docker pull amazonlinux@sha256:7e25084410d24fa4830e619f5331f018bd6e0ac5b53c47f2518a62d5e92a2cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220419.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:070a330b34fa85275ac40541a830d43b30aadc2a773648da9457dd6c003e47bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62368733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719a671add20f6fa0b850e3023e7d6115cdd2061ac571b1ec74f814cc2af8806`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 23 Apr 2022 01:20:58 GMT
ADD file:648f5c0af52d0f60f0c9312ed88484b5c47f37512d1da91cd171bfd6bd3eb693 in / 
# Sat, 23 Apr 2022 01:20:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d1651c8ca9fa2a1211ca3981a04760e4249b1ea5248c4650a768844c5bafa933`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 62.4 MB (62368733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220419.0-with-sources`

```console
$ docker pull amazonlinux@sha256:7c3adb037884d64f74753449315d0959969861102acaaa75e701e8e1d61bd2b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220419.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7b10e3edb3d85f719b0120d8fc02d6ae777e93b9996718df2caa826338c57a11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515018819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f74812e89dff5d7417f213101574bcafb217529538925d94bd5522e5df5ef86`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 23 Apr 2022 01:20:58 GMT
ADD file:648f5c0af52d0f60f0c9312ed88484b5c47f37512d1da91cd171bfd6bd3eb693 in / 
# Sat, 23 Apr 2022 01:20:58 GMT
CMD ["/bin/bash"]
# Sat, 23 Apr 2022 01:21:23 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3218b580f105e26d79916fd58a49937f9ae8cd25196a762d6e47d1d6c891e437.tar.gz"  && echo "c2cc764bbb63b9eaba23de4bd298faf993093ba4d8098eed411753d88dc9cde6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d1651c8ca9fa2a1211ca3981a04760e4249b1ea5248c4650a768844c5bafa933`  
		Last Modified: Sat, 23 Apr 2022 01:22:03 GMT  
		Size: 62.4 MB (62368733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0423df311996171a2ece9630104cac5b1ec4f5c5c3024bca6d9ce573f8f00f64`  
		Last Modified: Sat, 23 Apr 2022 01:22:32 GMT  
		Size: 452.7 MB (452650086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:620c4db9e2f373085b5a049e63ebc03b0b05b77335d3df9272532db09bce73a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:4ec4834e641a20cba296755081514de1811e97998825e465bc52ceaa45b3c5c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70553888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51c1f7cb94a260acd66ee97af80387320016f0ff007558c7aa895054dd4cc42`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:19:33 GMT
ADD file:8938ca932860236a5478568502c523de28f6fdb1844554dff09a9073e58e2d64 in / 
# Mon, 02 May 2022 23:19:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ea1ba8a91f0904c1d69fc8987dcf4d80e75a6f574e1b4a292e9be3e1b78f1def`  
		Last Modified: Mon, 02 May 2022 09:17:35 GMT  
		Size: 70.6 MB (70553888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2e9481a37ea86ce576879268b1c96ed1148d4a6c3f424e163f89fa1f03452409
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69103820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32e4a417fd4777e112a33c2e6a6f6884a2df374712167c1715ae3f5854c9816`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:41:36 GMT
ADD file:a7db6c0fde802c761f92fffcc7031a46d1d22f6bd270cfaf0f657e3f6ed18a98 in / 
# Mon, 02 May 2022 23:41:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:81baea72d1f94ce2611f8412d29ad6a68396cb5f45c7e2fe8f0dd9f3bb270744`  
		Last Modified: Mon, 02 May 2022 23:42:40 GMT  
		Size: 69.1 MB (69103820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:64a7fdc5af1fd9b724c7b28630a2aad58f82d08a3651eace866d061ed3781566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:698032efb39ccbab8dc9abc5dc3b57682f1da1b89aa8a60bed1e5fd24f87e7d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489262019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bacdbeb608c26f31936f6982745dade2ec6c8d386926a8d490da20af6de4a85`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:19:33 GMT
ADD file:8938ca932860236a5478568502c523de28f6fdb1844554dff09a9073e58e2d64 in / 
# Mon, 02 May 2022 23:19:34 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 23:19:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-30a96c4f6cb306f42c34e07a80efcfbe6980633a9ac34327014a87423221b673.tar.gz"  && echo "eb2de792ff0fb280db260db9b6f4c55b40e52059337fc4c1a293f79f2b4e45bf  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ea1ba8a91f0904c1d69fc8987dcf4d80e75a6f574e1b4a292e9be3e1b78f1def`  
		Last Modified: Mon, 02 May 2022 09:17:35 GMT  
		Size: 70.6 MB (70553888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39db4bfd73372833edec2c995c10e909ff279746b73b39bbb9a78a95ef9464a`  
		Last Modified: Mon, 02 May 2022 23:21:01 GMT  
		Size: 418.7 MB (418708131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ac9154ace84c95d05b14c2d4bfea4e43954b6e5f4d24a53ad86005883f8e68ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.8 MB (487811892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa0263e0ffa55f3b9062b5c556fc0f0e1869d31fcf2250385c602a8c083c1ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:41:36 GMT
ADD file:a7db6c0fde802c761f92fffcc7031a46d1d22f6bd270cfaf0f657e3f6ed18a98 in / 
# Mon, 02 May 2022 23:41:38 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 23:41:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-30a96c4f6cb306f42c34e07a80efcfbe6980633a9ac34327014a87423221b673.tar.gz"  && echo "eb2de792ff0fb280db260db9b6f4c55b40e52059337fc4c1a293f79f2b4e45bf  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:81baea72d1f94ce2611f8412d29ad6a68396cb5f45c7e2fe8f0dd9f3bb270744`  
		Last Modified: Mon, 02 May 2022 23:42:40 GMT  
		Size: 69.1 MB (69103820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee46a4843a1e40c260139a6926e48843ee1dc8fa172bb261e89f1ad679162268`  
		Last Modified: Mon, 02 May 2022 23:43:15 GMT  
		Size: 418.7 MB (418708072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220419.0`

```console
$ docker pull amazonlinux@sha256:620c4db9e2f373085b5a049e63ebc03b0b05b77335d3df9272532db09bce73a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220419.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:4ec4834e641a20cba296755081514de1811e97998825e465bc52ceaa45b3c5c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70553888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51c1f7cb94a260acd66ee97af80387320016f0ff007558c7aa895054dd4cc42`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:19:33 GMT
ADD file:8938ca932860236a5478568502c523de28f6fdb1844554dff09a9073e58e2d64 in / 
# Mon, 02 May 2022 23:19:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ea1ba8a91f0904c1d69fc8987dcf4d80e75a6f574e1b4a292e9be3e1b78f1def`  
		Last Modified: Mon, 02 May 2022 09:17:35 GMT  
		Size: 70.6 MB (70553888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220419.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2e9481a37ea86ce576879268b1c96ed1148d4a6c3f424e163f89fa1f03452409
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69103820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32e4a417fd4777e112a33c2e6a6f6884a2df374712167c1715ae3f5854c9816`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:41:36 GMT
ADD file:a7db6c0fde802c761f92fffcc7031a46d1d22f6bd270cfaf0f657e3f6ed18a98 in / 
# Mon, 02 May 2022 23:41:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:81baea72d1f94ce2611f8412d29ad6a68396cb5f45c7e2fe8f0dd9f3bb270744`  
		Last Modified: Mon, 02 May 2022 23:42:40 GMT  
		Size: 69.1 MB (69103820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220419.0-with-sources`

```console
$ docker pull amazonlinux@sha256:64a7fdc5af1fd9b724c7b28630a2aad58f82d08a3651eace866d061ed3781566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220419.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:698032efb39ccbab8dc9abc5dc3b57682f1da1b89aa8a60bed1e5fd24f87e7d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489262019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bacdbeb608c26f31936f6982745dade2ec6c8d386926a8d490da20af6de4a85`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:19:33 GMT
ADD file:8938ca932860236a5478568502c523de28f6fdb1844554dff09a9073e58e2d64 in / 
# Mon, 02 May 2022 23:19:34 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 23:19:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-30a96c4f6cb306f42c34e07a80efcfbe6980633a9ac34327014a87423221b673.tar.gz"  && echo "eb2de792ff0fb280db260db9b6f4c55b40e52059337fc4c1a293f79f2b4e45bf  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ea1ba8a91f0904c1d69fc8987dcf4d80e75a6f574e1b4a292e9be3e1b78f1def`  
		Last Modified: Mon, 02 May 2022 09:17:35 GMT  
		Size: 70.6 MB (70553888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39db4bfd73372833edec2c995c10e909ff279746b73b39bbb9a78a95ef9464a`  
		Last Modified: Mon, 02 May 2022 23:21:01 GMT  
		Size: 418.7 MB (418708131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220419.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ac9154ace84c95d05b14c2d4bfea4e43954b6e5f4d24a53ad86005883f8e68ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.8 MB (487811892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa0263e0ffa55f3b9062b5c556fc0f0e1869d31fcf2250385c602a8c083c1ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:41:36 GMT
ADD file:a7db6c0fde802c761f92fffcc7031a46d1d22f6bd270cfaf0f657e3f6ed18a98 in / 
# Mon, 02 May 2022 23:41:38 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 23:41:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-30a96c4f6cb306f42c34e07a80efcfbe6980633a9ac34327014a87423221b673.tar.gz"  && echo "eb2de792ff0fb280db260db9b6f4c55b40e52059337fc4c1a293f79f2b4e45bf  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:81baea72d1f94ce2611f8412d29ad6a68396cb5f45c7e2fe8f0dd9f3bb270744`  
		Last Modified: Mon, 02 May 2022 23:42:40 GMT  
		Size: 69.1 MB (69103820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee46a4843a1e40c260139a6926e48843ee1dc8fa172bb261e89f1ad679162268`  
		Last Modified: Mon, 02 May 2022 23:43:15 GMT  
		Size: 418.7 MB (418708072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:620c4db9e2f373085b5a049e63ebc03b0b05b77335d3df9272532db09bce73a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:4ec4834e641a20cba296755081514de1811e97998825e465bc52ceaa45b3c5c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70553888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51c1f7cb94a260acd66ee97af80387320016f0ff007558c7aa895054dd4cc42`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:19:33 GMT
ADD file:8938ca932860236a5478568502c523de28f6fdb1844554dff09a9073e58e2d64 in / 
# Mon, 02 May 2022 23:19:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ea1ba8a91f0904c1d69fc8987dcf4d80e75a6f574e1b4a292e9be3e1b78f1def`  
		Last Modified: Mon, 02 May 2022 09:17:35 GMT  
		Size: 70.6 MB (70553888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2e9481a37ea86ce576879268b1c96ed1148d4a6c3f424e163f89fa1f03452409
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69103820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32e4a417fd4777e112a33c2e6a6f6884a2df374712167c1715ae3f5854c9816`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:41:36 GMT
ADD file:a7db6c0fde802c761f92fffcc7031a46d1d22f6bd270cfaf0f657e3f6ed18a98 in / 
# Mon, 02 May 2022 23:41:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:81baea72d1f94ce2611f8412d29ad6a68396cb5f45c7e2fe8f0dd9f3bb270744`  
		Last Modified: Mon, 02 May 2022 23:42:40 GMT  
		Size: 69.1 MB (69103820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:64a7fdc5af1fd9b724c7b28630a2aad58f82d08a3651eace866d061ed3781566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:698032efb39ccbab8dc9abc5dc3b57682f1da1b89aa8a60bed1e5fd24f87e7d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489262019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bacdbeb608c26f31936f6982745dade2ec6c8d386926a8d490da20af6de4a85`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:19:33 GMT
ADD file:8938ca932860236a5478568502c523de28f6fdb1844554dff09a9073e58e2d64 in / 
# Mon, 02 May 2022 23:19:34 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 23:19:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-30a96c4f6cb306f42c34e07a80efcfbe6980633a9ac34327014a87423221b673.tar.gz"  && echo "eb2de792ff0fb280db260db9b6f4c55b40e52059337fc4c1a293f79f2b4e45bf  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ea1ba8a91f0904c1d69fc8987dcf4d80e75a6f574e1b4a292e9be3e1b78f1def`  
		Last Modified: Mon, 02 May 2022 09:17:35 GMT  
		Size: 70.6 MB (70553888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39db4bfd73372833edec2c995c10e909ff279746b73b39bbb9a78a95ef9464a`  
		Last Modified: Mon, 02 May 2022 23:21:01 GMT  
		Size: 418.7 MB (418708131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:ac9154ace84c95d05b14c2d4bfea4e43954b6e5f4d24a53ad86005883f8e68ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.8 MB (487811892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa0263e0ffa55f3b9062b5c556fc0f0e1869d31fcf2250385c602a8c083c1ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 02 May 2022 23:41:36 GMT
ADD file:a7db6c0fde802c761f92fffcc7031a46d1d22f6bd270cfaf0f657e3f6ed18a98 in / 
# Mon, 02 May 2022 23:41:38 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 23:41:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-30a96c4f6cb306f42c34e07a80efcfbe6980633a9ac34327014a87423221b673.tar.gz"  && echo "eb2de792ff0fb280db260db9b6f4c55b40e52059337fc4c1a293f79f2b4e45bf  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:81baea72d1f94ce2611f8412d29ad6a68396cb5f45c7e2fe8f0dd9f3bb270744`  
		Last Modified: Mon, 02 May 2022 23:42:40 GMT  
		Size: 69.1 MB (69103820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee46a4843a1e40c260139a6926e48843ee1dc8fa172bb261e89f1ad679162268`  
		Last Modified: Mon, 02 May 2022 23:43:15 GMT  
		Size: 418.7 MB (418708072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:54f592d954725ce989af5ed5fb49e35ab2b1f1d830ee3f1f79b58ed75a631f64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1301cc9f889f21dc45733df9e58034ac1c318202b4b0f0a08d88b3fdc03004de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62265199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365842604a8b06c7c6dcb1ead27ee7297138603dc36dd4a64fe0421100256334`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:19:57 GMT
ADD file:4eb88d9d977dadb40c630d693a07ca066069b30b9751b7a421dfb4ba0b99d862 in / 
# Thu, 21 Apr 2022 22:19:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ac1397dc8419bf1767b60a5cc5849b7130406030581d4542e48965801c303a70`  
		Last Modified: Thu, 21 Apr 2022 22:08:36 GMT  
		Size: 62.3 MB (62265199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2249ff9b9983e5b9983c560645d6378f825827723b4a8c8a30ccb6d8cb661276
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63888157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:583d35ff5db28103719d2359a7e631acc8e85896a9ca9fb45f99fd36511c1aae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:57:49 GMT
ADD file:76e1ee72575f50a75573a46483631e239d3b6afda9fdd53086883bd03db5364b in / 
# Thu, 21 Apr 2022 22:57:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:86bcd0b49e3391c117b5e27756fdf585aadc1a7b9054d19af0faa050839a6633`  
		Last Modified: Thu, 21 Apr 2022 22:59:02 GMT  
		Size: 63.9 MB (63888157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:c2f343c1353778866e90fba96b5b6173b255f07d302de7c0703c9c67d1c863f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:67fd44e1ca29a3c41ea875774083e64f218643232b1f5f27dfb1b1e4b6aeebf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485656205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511c70976d4f4738c09199e01633142618f58f7bc2345948fa514aba7741d28e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:19:57 GMT
ADD file:4eb88d9d977dadb40c630d693a07ca066069b30b9751b7a421dfb4ba0b99d862 in / 
# Thu, 21 Apr 2022 22:19:58 GMT
CMD ["/bin/bash"]
# Thu, 21 Apr 2022 22:20:24 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-915f4823664b0d5efa5a9e17372f52c1e32718dcd0045d286495168c62f27bf6.tar.gz"  && echo "ddee5f71296afcb2dc85200f657f30688a3edb91a3e317592c02d9b387c62d5b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ac1397dc8419bf1767b60a5cc5849b7130406030581d4542e48965801c303a70`  
		Last Modified: Thu, 21 Apr 2022 22:08:36 GMT  
		Size: 62.3 MB (62265199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf04fc591da032b75c5a1e2f399e07e93a1b66b3bc75b07fe457ede25a29d9d`  
		Last Modified: Thu, 21 Apr 2022 22:21:31 GMT  
		Size: 423.4 MB (423391006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9ef53f86fd3105e8d6ed9465463739e3c672d0fb995722e7a7a0abf09bd2954b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487279116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a0bc6da757fa79443ed42fd5cf1b1909702466a8a507cfc78ca9f1ea291a09`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:57:49 GMT
ADD file:76e1ee72575f50a75573a46483631e239d3b6afda9fdd53086883bd03db5364b in / 
# Thu, 21 Apr 2022 22:57:51 GMT
CMD ["/bin/bash"]
# Thu, 21 Apr 2022 22:58:15 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-915f4823664b0d5efa5a9e17372f52c1e32718dcd0045d286495168c62f27bf6.tar.gz"  && echo "ddee5f71296afcb2dc85200f657f30688a3edb91a3e317592c02d9b387c62d5b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:86bcd0b49e3391c117b5e27756fdf585aadc1a7b9054d19af0faa050839a6633`  
		Last Modified: Thu, 21 Apr 2022 22:59:02 GMT  
		Size: 63.9 MB (63888157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17307b92b5f720ad82dc04ee1d549790061ada9c458c29252ff0e64f85017078`  
		Last Modified: Thu, 21 Apr 2022 22:59:56 GMT  
		Size: 423.4 MB (423390959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
