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
$ docker pull amazonlinux@sha256:246ef631c75ea83005889621119fd5cc9cbb5500e193707c38b6c060d597a146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:5ca9e45da788e7bac100dffaf45645cea5af68d46f62144f683c0434e14fd586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62291142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdeb69c57ad20820ceb442c918b35228a6c9d04d6458768fdf4e86429cbccca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b1377309830b143f16246542ac234b8b0b9251533954bfb9d3ffd79e2c199901
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a0df532d4a93ede0e0da29817f5dfdfb9c6653e22e32388de3149618d47cef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:f66f05473f90aa6e14ac926ec03d61af16828a2ff9205fbfa1d3713670b0c166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9a3fbba8f30fbd72a0aa0116fd0ef46e8af25d260d01073c266347f116f20399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485712608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6855b0eeeef206786c8c7ac97e546f8677b9d18b2fead70262d5cebc674f86d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 23:19:53 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0efe039696303bb91bcd3177af472d1339e2e4cd62297fabd75e1763b9bcb9`  
		Last Modified: Tue, 03 May 2022 23:21:15 GMT  
		Size: 423.4 MB (423421466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:124eb9a22c4bd8d59ea311f776bae5213d1e66db6103732c2c10741bb263f459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487323598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671abfcb4f4c6d925fbecf84883a36ca87a0e7e8aa40bc10b0c3a1678f2b1168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 22:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189fd58a2d5dc106fd8a0dee23c67eaa14f4c78c0e8fecb154e921df7a05540e`  
		Last Modified: Tue, 03 May 2022 22:41:23 GMT  
		Size: 423.4 MB (423421419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220426.0`

```console
$ docker pull amazonlinux@sha256:246ef631c75ea83005889621119fd5cc9cbb5500e193707c38b6c060d597a146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220426.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:5ca9e45da788e7bac100dffaf45645cea5af68d46f62144f683c0434e14fd586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62291142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdeb69c57ad20820ceb442c918b35228a6c9d04d6458768fdf4e86429cbccca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220426.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b1377309830b143f16246542ac234b8b0b9251533954bfb9d3ffd79e2c199901
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a0df532d4a93ede0e0da29817f5dfdfb9c6653e22e32388de3149618d47cef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220426.0-with-sources`

```console
$ docker pull amazonlinux@sha256:f66f05473f90aa6e14ac926ec03d61af16828a2ff9205fbfa1d3713670b0c166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220426.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9a3fbba8f30fbd72a0aa0116fd0ef46e8af25d260d01073c266347f116f20399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485712608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6855b0eeeef206786c8c7ac97e546f8677b9d18b2fead70262d5cebc674f86d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 23:19:53 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0efe039696303bb91bcd3177af472d1339e2e4cd62297fabd75e1763b9bcb9`  
		Last Modified: Tue, 03 May 2022 23:21:15 GMT  
		Size: 423.4 MB (423421466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220426.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:124eb9a22c4bd8d59ea311f776bae5213d1e66db6103732c2c10741bb263f459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487323598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671abfcb4f4c6d925fbecf84883a36ca87a0e7e8aa40bc10b0c3a1678f2b1168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 22:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189fd58a2d5dc106fd8a0dee23c67eaa14f4c78c0e8fecb154e921df7a05540e`  
		Last Modified: Tue, 03 May 2022 22:41:23 GMT  
		Size: 423.4 MB (423421419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull amazonlinux@sha256:246ef631c75ea83005889621119fd5cc9cbb5500e193707c38b6c060d597a146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:5ca9e45da788e7bac100dffaf45645cea5af68d46f62144f683c0434e14fd586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62291142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdeb69c57ad20820ceb442c918b35228a6c9d04d6458768fdf4e86429cbccca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b1377309830b143f16246542ac234b8b0b9251533954bfb9d3ffd79e2c199901
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a0df532d4a93ede0e0da29817f5dfdfb9c6653e22e32388de3149618d47cef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:f66f05473f90aa6e14ac926ec03d61af16828a2ff9205fbfa1d3713670b0c166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9a3fbba8f30fbd72a0aa0116fd0ef46e8af25d260d01073c266347f116f20399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485712608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6855b0eeeef206786c8c7ac97e546f8677b9d18b2fead70262d5cebc674f86d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 23:19:53 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0efe039696303bb91bcd3177af472d1339e2e4cd62297fabd75e1763b9bcb9`  
		Last Modified: Tue, 03 May 2022 23:21:15 GMT  
		Size: 423.4 MB (423421466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:124eb9a22c4bd8d59ea311f776bae5213d1e66db6103732c2c10741bb263f459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487323598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671abfcb4f4c6d925fbecf84883a36ca87a0e7e8aa40bc10b0c3a1678f2b1168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 22:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189fd58a2d5dc106fd8a0dee23c67eaa14f4c78c0e8fecb154e921df7a05540e`  
		Last Modified: Tue, 03 May 2022 22:41:23 GMT  
		Size: 423.4 MB (423421419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
