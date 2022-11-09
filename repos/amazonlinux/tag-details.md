<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20221004.0`](#amazonlinux20202210040)
-	[`amazonlinux:2.0.20221004.0-with-sources`](#amazonlinux20202210040-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20221018.0`](#amazonlinux2018030202210180)
-	[`amazonlinux:2018.03.0.20221018.0-with-sources`](#amazonlinux2018030202210180-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20221101.0`](#amazonlinux20220202211010)
-	[`amazonlinux:2022.0.20221101.0-with-sources`](#amazonlinux20220202211010-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:eb90fa0fd56cf880979f65bea71c7eb281c7dc89a488d7092ead33d2b9b2e46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e8df9dda3c5292dd7ef9a88d4f48f137777d10a66a5092c1fcca487e68f9d646
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62313541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba5363925e500c1013b0ec6e6b7a360d9c5fce273cdde1c66cfbe207d2331e59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 09 Nov 2022 00:20:14 GMT
ADD file:0410dbf81388508f909ade34c62fad7fec8bf5bab19b58a8a35c41acee8b4740 in / 
# Wed, 09 Nov 2022 00:20:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:239d83e9c6fb7a202ec4084ddd8523b8c6adecb0018abbeb8e5527303640c8d9`  
		Last Modified: Wed, 09 Nov 2022 00:21:28 GMT  
		Size: 62.3 MB (62313541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:645b31167fc038f0e7adcdf2ff61ade80b5196df1b28db447dd60d837e963062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e16ebcdcc59bbaec60b9d8a84b0268f293bfd4a937be37c2ac2c1bbd2d851bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515019772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbce77f59d1e6d589eafa0793b60aa0bb0b16dd1eec9459f1c2dd975d4e7ef69`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 09 Nov 2022 00:20:14 GMT
ADD file:0410dbf81388508f909ade34c62fad7fec8bf5bab19b58a8a35c41acee8b4740 in / 
# Wed, 09 Nov 2022 00:20:14 GMT
CMD ["/bin/bash"]
# Wed, 09 Nov 2022 00:20:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6187381cfff74a5e739858bf043ff837ea10f446423f99fdb7c9af84c17343a2.tar.gz"     && echo "48bbea24b4a488fe06936dd9651cde99e66dc16ee4c06feaa246edc9393c1cb5  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:239d83e9c6fb7a202ec4084ddd8523b8c6adecb0018abbeb8e5527303640c8d9`  
		Last Modified: Wed, 09 Nov 2022 00:21:28 GMT  
		Size: 62.3 MB (62313541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140305c0ab9b02db4b457cd8851da53989035af98c8c9e145649884d289b9faa`  
		Last Modified: Wed, 09 Nov 2022 00:21:58 GMT  
		Size: 452.7 MB (452706231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:f0ad031d65bf6cd219d8621d2a304d884c6a809ca2b20855eac371df92f4fcaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:37b666a59e80b8b0c78f8e3396c944fe4cf0a1ba27e3d6d93324d3f57a2cfeb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62306642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24608685b402b0a8ac1bdc9a1f7c662e5b88dd4620037bea8d7501cd3b2508bc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:df60b5cd5325466f3a8b3ccb300ed5dc16627cbc84b4de3472a5dcc4ea2656fa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63919869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5514655128c44a2bb0b46008b034780a5cfc9090cb31e0d4c866e784602587a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:06 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Wed, 26 Oct 2022 15:27:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:d8317c7ade584beb412079366b679f659198063efa81c3ba17d9b8217b35a10a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:18d4254908fe549a3b74fe48afee88802d42765cc8cdad730a1d31f869d6065d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486382082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1372932df6c9127867ac9e8a7db0a8f25d0e776f7da5a33592582813cce66cdd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 00:20:21 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae837e2df6db6c81612d2da73f641c413ed66985e004a9a6565edcdb2b757a12`  
		Last Modified: Fri, 21 Oct 2022 00:21:31 GMT  
		Size: 424.1 MB (424075440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:666035ad6bcdcb3acd33d5a1149aa9f33326ba6a3d37cefdd07aa795400d2e38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487995306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:724f4723c160d54b79d767819020361b49089bc3383b30d244c7a5e28b8e50ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:06 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Wed, 26 Oct 2022 15:27:06 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 15:27:30 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c2dbbe36f82b868eeba9da518a5cd14946071330d0876e061dfde90df696`  
		Last Modified: Wed, 26 Oct 2022 15:28:41 GMT  
		Size: 424.1 MB (424075437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20221004.0`

```console
$ docker pull amazonlinux@sha256:f0ad031d65bf6cd219d8621d2a304d884c6a809ca2b20855eac371df92f4fcaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20221004.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:37b666a59e80b8b0c78f8e3396c944fe4cf0a1ba27e3d6d93324d3f57a2cfeb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62306642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24608685b402b0a8ac1bdc9a1f7c662e5b88dd4620037bea8d7501cd3b2508bc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20221004.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:df60b5cd5325466f3a8b3ccb300ed5dc16627cbc84b4de3472a5dcc4ea2656fa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63919869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5514655128c44a2bb0b46008b034780a5cfc9090cb31e0d4c866e784602587a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:06 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Wed, 26 Oct 2022 15:27:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20221004.0-with-sources`

```console
$ docker pull amazonlinux@sha256:d8317c7ade584beb412079366b679f659198063efa81c3ba17d9b8217b35a10a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20221004.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:18d4254908fe549a3b74fe48afee88802d42765cc8cdad730a1d31f869d6065d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486382082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1372932df6c9127867ac9e8a7db0a8f25d0e776f7da5a33592582813cce66cdd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 00:20:21 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae837e2df6db6c81612d2da73f641c413ed66985e004a9a6565edcdb2b757a12`  
		Last Modified: Fri, 21 Oct 2022 00:21:31 GMT  
		Size: 424.1 MB (424075440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20221004.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:666035ad6bcdcb3acd33d5a1149aa9f33326ba6a3d37cefdd07aa795400d2e38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487995306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:724f4723c160d54b79d767819020361b49089bc3383b30d244c7a5e28b8e50ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:06 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Wed, 26 Oct 2022 15:27:06 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 15:27:30 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c2dbbe36f82b868eeba9da518a5cd14946071330d0876e061dfde90df696`  
		Last Modified: Wed, 26 Oct 2022 15:28:41 GMT  
		Size: 424.1 MB (424075437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:eb90fa0fd56cf880979f65bea71c7eb281c7dc89a488d7092ead33d2b9b2e46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e8df9dda3c5292dd7ef9a88d4f48f137777d10a66a5092c1fcca487e68f9d646
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62313541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba5363925e500c1013b0ec6e6b7a360d9c5fce273cdde1c66cfbe207d2331e59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 09 Nov 2022 00:20:14 GMT
ADD file:0410dbf81388508f909ade34c62fad7fec8bf5bab19b58a8a35c41acee8b4740 in / 
# Wed, 09 Nov 2022 00:20:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:239d83e9c6fb7a202ec4084ddd8523b8c6adecb0018abbeb8e5527303640c8d9`  
		Last Modified: Wed, 09 Nov 2022 00:21:28 GMT  
		Size: 62.3 MB (62313541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:645b31167fc038f0e7adcdf2ff61ade80b5196df1b28db447dd60d837e963062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e16ebcdcc59bbaec60b9d8a84b0268f293bfd4a937be37c2ac2c1bbd2d851bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515019772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbce77f59d1e6d589eafa0793b60aa0bb0b16dd1eec9459f1c2dd975d4e7ef69`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 09 Nov 2022 00:20:14 GMT
ADD file:0410dbf81388508f909ade34c62fad7fec8bf5bab19b58a8a35c41acee8b4740 in / 
# Wed, 09 Nov 2022 00:20:14 GMT
CMD ["/bin/bash"]
# Wed, 09 Nov 2022 00:20:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6187381cfff74a5e739858bf043ff837ea10f446423f99fdb7c9af84c17343a2.tar.gz"     && echo "48bbea24b4a488fe06936dd9651cde99e66dc16ee4c06feaa246edc9393c1cb5  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:239d83e9c6fb7a202ec4084ddd8523b8c6adecb0018abbeb8e5527303640c8d9`  
		Last Modified: Wed, 09 Nov 2022 00:21:28 GMT  
		Size: 62.3 MB (62313541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140305c0ab9b02db4b457cd8851da53989035af98c8c9e145649884d289b9faa`  
		Last Modified: Wed, 09 Nov 2022 00:21:58 GMT  
		Size: 452.7 MB (452706231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20221018.0`

```console
$ docker pull amazonlinux@sha256:eb90fa0fd56cf880979f65bea71c7eb281c7dc89a488d7092ead33d2b9b2e46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20221018.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e8df9dda3c5292dd7ef9a88d4f48f137777d10a66a5092c1fcca487e68f9d646
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62313541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba5363925e500c1013b0ec6e6b7a360d9c5fce273cdde1c66cfbe207d2331e59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 09 Nov 2022 00:20:14 GMT
ADD file:0410dbf81388508f909ade34c62fad7fec8bf5bab19b58a8a35c41acee8b4740 in / 
# Wed, 09 Nov 2022 00:20:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:239d83e9c6fb7a202ec4084ddd8523b8c6adecb0018abbeb8e5527303640c8d9`  
		Last Modified: Wed, 09 Nov 2022 00:21:28 GMT  
		Size: 62.3 MB (62313541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20221018.0-with-sources`

```console
$ docker pull amazonlinux@sha256:645b31167fc038f0e7adcdf2ff61ade80b5196df1b28db447dd60d837e963062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20221018.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e16ebcdcc59bbaec60b9d8a84b0268f293bfd4a937be37c2ac2c1bbd2d851bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515019772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbce77f59d1e6d589eafa0793b60aa0bb0b16dd1eec9459f1c2dd975d4e7ef69`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 09 Nov 2022 00:20:14 GMT
ADD file:0410dbf81388508f909ade34c62fad7fec8bf5bab19b58a8a35c41acee8b4740 in / 
# Wed, 09 Nov 2022 00:20:14 GMT
CMD ["/bin/bash"]
# Wed, 09 Nov 2022 00:20:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6187381cfff74a5e739858bf043ff837ea10f446423f99fdb7c9af84c17343a2.tar.gz"     && echo "48bbea24b4a488fe06936dd9651cde99e66dc16ee4c06feaa246edc9393c1cb5  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:239d83e9c6fb7a202ec4084ddd8523b8c6adecb0018abbeb8e5527303640c8d9`  
		Last Modified: Wed, 09 Nov 2022 00:21:28 GMT  
		Size: 62.3 MB (62313541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140305c0ab9b02db4b457cd8851da53989035af98c8c9e145649884d289b9faa`  
		Last Modified: Wed, 09 Nov 2022 00:21:58 GMT  
		Size: 452.7 MB (452706231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:98501b204b89ad4b5eb08ab06f2f7f82edc3fa637ba61ab4015d8b0856865b52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:21e0ad332ee2c3723b20357f76829cda81da6ff6e2630eed6c56658514a75cd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76310d45eddd6a35aab56db52088c8936e5507e2028d51b07da7ecc0ddebf42c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:26 GMT
ADD file:541cbb916857290067c17f8f5718a02004fa3ade45da9cd68db6a3fbec9191a6 in / 
# Tue, 01 Nov 2022 23:11:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1f61030557f6b1b4adb79deb32494aecd38af05ed90a5d54900eea80eedc3bb`  
		Last Modified: Tue, 01 Nov 2022 23:12:19 GMT  
		Size: 57.7 MB (57657867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4ef67a181bdcff39e952bb9251c0a2ffeef76b11a8f97e4a6f9fb8d9cf135136
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56505867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4d88c9fe91d0f351545f815433c3beb52cff87f1686557df9eec87f4e4acdf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:12 GMT
ADD file:a96a24d7338f7e441a7666f0001096f24674170b376588f39095734b91d9dfed in / 
# Tue, 01 Nov 2022 23:11:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9f53c5402c7b18b2658ebb93a03c882a5ca1212112c795f5d4a3c561ea6fcd2f`  
		Last Modified: Tue, 01 Nov 2022 23:12:05 GMT  
		Size: 56.5 MB (56505867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:b929906fa10216314b0f1e2dc978a65b9874c515479c0651bcbd4728afb4ad8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:47b2413f80d9392dbbdabb09d40ede432afd8dc11a638cc2176c8f4399ad3f87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.8 MB (387791955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419b95c0aecedd809286c2f73a221ceed144a188f5ee55079c1cef975eba20a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:26 GMT
ADD file:541cbb916857290067c17f8f5718a02004fa3ade45da9cd68db6a3fbec9191a6 in / 
# Tue, 01 Nov 2022 23:11:26 GMT
CMD ["/bin/bash"]
# Tue, 01 Nov 2022 23:11:43 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9017832186b37ba807d501395b1ecd1dee072363f2dbf07cd660b9c6901e23d5.tar.gz"     && echo "e381f621dad069a24ac99c48de67decd4a83465925c195fd186bb3ed587d7a9c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b1f61030557f6b1b4adb79deb32494aecd38af05ed90a5d54900eea80eedc3bb`  
		Last Modified: Tue, 01 Nov 2022 23:12:19 GMT  
		Size: 57.7 MB (57657867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfa8588296ea9cc5617b6ef566ee485a036bd55235e0d28bec7633d17a17f42`  
		Last Modified: Tue, 01 Nov 2022 23:12:44 GMT  
		Size: 330.1 MB (330134088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6468c6cf7df684bb1ae74c398a80f81752d6683e98006549905dc511018e6dbd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.6 MB (386639956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bcdcbc0090700ece3f1f96dee45ce818350cf95282dd1d4f08f0f1d47d55d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:12 GMT
ADD file:a96a24d7338f7e441a7666f0001096f24674170b376588f39095734b91d9dfed in / 
# Tue, 01 Nov 2022 23:11:13 GMT
CMD ["/bin/bash"]
# Tue, 01 Nov 2022 23:11:32 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9017832186b37ba807d501395b1ecd1dee072363f2dbf07cd660b9c6901e23d5.tar.gz"     && echo "e381f621dad069a24ac99c48de67decd4a83465925c195fd186bb3ed587d7a9c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9f53c5402c7b18b2658ebb93a03c882a5ca1212112c795f5d4a3c561ea6fcd2f`  
		Last Modified: Tue, 01 Nov 2022 23:12:05 GMT  
		Size: 56.5 MB (56505867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e1358755b392436e218dd02e545f2712370f5328f9d4542512845f4059fc5b`  
		Last Modified: Tue, 01 Nov 2022 23:12:28 GMT  
		Size: 330.1 MB (330134089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20221101.0`

```console
$ docker pull amazonlinux@sha256:98501b204b89ad4b5eb08ab06f2f7f82edc3fa637ba61ab4015d8b0856865b52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20221101.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:21e0ad332ee2c3723b20357f76829cda81da6ff6e2630eed6c56658514a75cd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76310d45eddd6a35aab56db52088c8936e5507e2028d51b07da7ecc0ddebf42c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:26 GMT
ADD file:541cbb916857290067c17f8f5718a02004fa3ade45da9cd68db6a3fbec9191a6 in / 
# Tue, 01 Nov 2022 23:11:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1f61030557f6b1b4adb79deb32494aecd38af05ed90a5d54900eea80eedc3bb`  
		Last Modified: Tue, 01 Nov 2022 23:12:19 GMT  
		Size: 57.7 MB (57657867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20221101.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4ef67a181bdcff39e952bb9251c0a2ffeef76b11a8f97e4a6f9fb8d9cf135136
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56505867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4d88c9fe91d0f351545f815433c3beb52cff87f1686557df9eec87f4e4acdf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:12 GMT
ADD file:a96a24d7338f7e441a7666f0001096f24674170b376588f39095734b91d9dfed in / 
# Tue, 01 Nov 2022 23:11:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9f53c5402c7b18b2658ebb93a03c882a5ca1212112c795f5d4a3c561ea6fcd2f`  
		Last Modified: Tue, 01 Nov 2022 23:12:05 GMT  
		Size: 56.5 MB (56505867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20221101.0-with-sources`

```console
$ docker pull amazonlinux@sha256:b929906fa10216314b0f1e2dc978a65b9874c515479c0651bcbd4728afb4ad8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20221101.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:47b2413f80d9392dbbdabb09d40ede432afd8dc11a638cc2176c8f4399ad3f87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.8 MB (387791955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419b95c0aecedd809286c2f73a221ceed144a188f5ee55079c1cef975eba20a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:26 GMT
ADD file:541cbb916857290067c17f8f5718a02004fa3ade45da9cd68db6a3fbec9191a6 in / 
# Tue, 01 Nov 2022 23:11:26 GMT
CMD ["/bin/bash"]
# Tue, 01 Nov 2022 23:11:43 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9017832186b37ba807d501395b1ecd1dee072363f2dbf07cd660b9c6901e23d5.tar.gz"     && echo "e381f621dad069a24ac99c48de67decd4a83465925c195fd186bb3ed587d7a9c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b1f61030557f6b1b4adb79deb32494aecd38af05ed90a5d54900eea80eedc3bb`  
		Last Modified: Tue, 01 Nov 2022 23:12:19 GMT  
		Size: 57.7 MB (57657867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfa8588296ea9cc5617b6ef566ee485a036bd55235e0d28bec7633d17a17f42`  
		Last Modified: Tue, 01 Nov 2022 23:12:44 GMT  
		Size: 330.1 MB (330134088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20221101.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6468c6cf7df684bb1ae74c398a80f81752d6683e98006549905dc511018e6dbd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.6 MB (386639956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bcdcbc0090700ece3f1f96dee45ce818350cf95282dd1d4f08f0f1d47d55d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:12 GMT
ADD file:a96a24d7338f7e441a7666f0001096f24674170b376588f39095734b91d9dfed in / 
# Tue, 01 Nov 2022 23:11:13 GMT
CMD ["/bin/bash"]
# Tue, 01 Nov 2022 23:11:32 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9017832186b37ba807d501395b1ecd1dee072363f2dbf07cd660b9c6901e23d5.tar.gz"     && echo "e381f621dad069a24ac99c48de67decd4a83465925c195fd186bb3ed587d7a9c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9f53c5402c7b18b2658ebb93a03c882a5ca1212112c795f5d4a3c561ea6fcd2f`  
		Last Modified: Tue, 01 Nov 2022 23:12:05 GMT  
		Size: 56.5 MB (56505867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e1358755b392436e218dd02e545f2712370f5328f9d4542512845f4059fc5b`  
		Last Modified: Tue, 01 Nov 2022 23:12:28 GMT  
		Size: 330.1 MB (330134089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:98501b204b89ad4b5eb08ab06f2f7f82edc3fa637ba61ab4015d8b0856865b52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:21e0ad332ee2c3723b20357f76829cda81da6ff6e2630eed6c56658514a75cd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76310d45eddd6a35aab56db52088c8936e5507e2028d51b07da7ecc0ddebf42c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:26 GMT
ADD file:541cbb916857290067c17f8f5718a02004fa3ade45da9cd68db6a3fbec9191a6 in / 
# Tue, 01 Nov 2022 23:11:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1f61030557f6b1b4adb79deb32494aecd38af05ed90a5d54900eea80eedc3bb`  
		Last Modified: Tue, 01 Nov 2022 23:12:19 GMT  
		Size: 57.7 MB (57657867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4ef67a181bdcff39e952bb9251c0a2ffeef76b11a8f97e4a6f9fb8d9cf135136
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56505867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4d88c9fe91d0f351545f815433c3beb52cff87f1686557df9eec87f4e4acdf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:12 GMT
ADD file:a96a24d7338f7e441a7666f0001096f24674170b376588f39095734b91d9dfed in / 
# Tue, 01 Nov 2022 23:11:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9f53c5402c7b18b2658ebb93a03c882a5ca1212112c795f5d4a3c561ea6fcd2f`  
		Last Modified: Tue, 01 Nov 2022 23:12:05 GMT  
		Size: 56.5 MB (56505867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:b929906fa10216314b0f1e2dc978a65b9874c515479c0651bcbd4728afb4ad8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:47b2413f80d9392dbbdabb09d40ede432afd8dc11a638cc2176c8f4399ad3f87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.8 MB (387791955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419b95c0aecedd809286c2f73a221ceed144a188f5ee55079c1cef975eba20a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:26 GMT
ADD file:541cbb916857290067c17f8f5718a02004fa3ade45da9cd68db6a3fbec9191a6 in / 
# Tue, 01 Nov 2022 23:11:26 GMT
CMD ["/bin/bash"]
# Tue, 01 Nov 2022 23:11:43 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9017832186b37ba807d501395b1ecd1dee072363f2dbf07cd660b9c6901e23d5.tar.gz"     && echo "e381f621dad069a24ac99c48de67decd4a83465925c195fd186bb3ed587d7a9c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:b1f61030557f6b1b4adb79deb32494aecd38af05ed90a5d54900eea80eedc3bb`  
		Last Modified: Tue, 01 Nov 2022 23:12:19 GMT  
		Size: 57.7 MB (57657867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfa8588296ea9cc5617b6ef566ee485a036bd55235e0d28bec7633d17a17f42`  
		Last Modified: Tue, 01 Nov 2022 23:12:44 GMT  
		Size: 330.1 MB (330134088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6468c6cf7df684bb1ae74c398a80f81752d6683e98006549905dc511018e6dbd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.6 MB (386639956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bcdcbc0090700ece3f1f96dee45ce818350cf95282dd1d4f08f0f1d47d55d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:12 GMT
ADD file:a96a24d7338f7e441a7666f0001096f24674170b376588f39095734b91d9dfed in / 
# Tue, 01 Nov 2022 23:11:13 GMT
CMD ["/bin/bash"]
# Tue, 01 Nov 2022 23:11:32 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9017832186b37ba807d501395b1ecd1dee072363f2dbf07cd660b9c6901e23d5.tar.gz"     && echo "e381f621dad069a24ac99c48de67decd4a83465925c195fd186bb3ed587d7a9c  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9f53c5402c7b18b2658ebb93a03c882a5ca1212112c795f5d4a3c561ea6fcd2f`  
		Last Modified: Tue, 01 Nov 2022 23:12:05 GMT  
		Size: 56.5 MB (56505867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e1358755b392436e218dd02e545f2712370f5328f9d4542512845f4059fc5b`  
		Last Modified: Tue, 01 Nov 2022 23:12:28 GMT  
		Size: 330.1 MB (330134089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:f0ad031d65bf6cd219d8621d2a304d884c6a809ca2b20855eac371df92f4fcaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:37b666a59e80b8b0c78f8e3396c944fe4cf0a1ba27e3d6d93324d3f57a2cfeb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62306642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24608685b402b0a8ac1bdc9a1f7c662e5b88dd4620037bea8d7501cd3b2508bc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:df60b5cd5325466f3a8b3ccb300ed5dc16627cbc84b4de3472a5dcc4ea2656fa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63919869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5514655128c44a2bb0b46008b034780a5cfc9090cb31e0d4c866e784602587a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:06 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Wed, 26 Oct 2022 15:27:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:d8317c7ade584beb412079366b679f659198063efa81c3ba17d9b8217b35a10a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:18d4254908fe549a3b74fe48afee88802d42765cc8cdad730a1d31f869d6065d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486382082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1372932df6c9127867ac9e8a7db0a8f25d0e776f7da5a33592582813cce66cdd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 00:20:21 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae837e2df6db6c81612d2da73f641c413ed66985e004a9a6565edcdb2b757a12`  
		Last Modified: Fri, 21 Oct 2022 00:21:31 GMT  
		Size: 424.1 MB (424075440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:666035ad6bcdcb3acd33d5a1149aa9f33326ba6a3d37cefdd07aa795400d2e38
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487995306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:724f4723c160d54b79d767819020361b49089bc3383b30d244c7a5e28b8e50ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:06 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Wed, 26 Oct 2022 15:27:06 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 15:27:30 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c2dbbe36f82b868eeba9da518a5cd14946071330d0876e061dfde90df696`  
		Last Modified: Wed, 26 Oct 2022 15:28:41 GMT  
		Size: 424.1 MB (424075437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
