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
-	[`amazonlinux:2018.03.0.20220907.3`](#amazonlinux2018030202209073)
-	[`amazonlinux:2018.03.0.20220907.3-with-sources`](#amazonlinux2018030202209073-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20221019.4`](#amazonlinux20220202210194)
-	[`amazonlinux:2022.0.20221019.4-with-sources`](#amazonlinux20220202210194-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:76029546e00113df116bb8ee36325dc5899b400da548b56e0fc2ec8ebd956b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3ab248170c3e4249b1a92534d8f8cb930da18a121812b2e3278ec8c2d9294485
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62306153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aeea0c5057a2c9bd77f4eadcb14a93ebc261bda8c9514fcdb762a0d36cbe5fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 23:19:39 GMT
ADD file:11f2036244afbd13a8d3e9654c8d3f3c99ab9e95ef31da94eed913ef504d6402 in / 
# Tue, 18 Oct 2022 23:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:090d64299c33248904e88674db63d2249fd29a5edf13fb417725a29c0819b946`  
		Last Modified: Tue, 18 Oct 2022 23:20:40 GMT  
		Size: 62.3 MB (62306153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:045dc0239192ac57f1fdc0a9cbb7a439e304f5bf5889256df234b1f5b23e23f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9b86385f3bc215268006627fbd6c23ec51b18756ea5b4e068ae8900c16af9253
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515011060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27784d8c4b05aa4fbb3556fe55ae176abb2c16639f09575e40dd65f617d9cc57`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 23:19:39 GMT
ADD file:11f2036244afbd13a8d3e9654c8d3f3c99ab9e95ef31da94eed913ef504d6402 in / 
# Tue, 18 Oct 2022 23:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 23:20:02 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6ba2180923a2f0b8f246ae7be3845522efffb9448264973c7b5f811296052d2c.tar.gz"     && echo "61c3e2a1535708dda90f5aa3cc856487b4950505f5c23e2e157933ced6a29670  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:090d64299c33248904e88674db63d2249fd29a5edf13fb417725a29c0819b946`  
		Last Modified: Tue, 18 Oct 2022 23:20:40 GMT  
		Size: 62.3 MB (62306153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc7431b327c65a3885610990e3515567e38c205976f395c3964df42dd030c5`  
		Last Modified: Tue, 18 Oct 2022 23:21:09 GMT  
		Size: 452.7 MB (452704907 bytes)  
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
$ docker pull amazonlinux@sha256:76029546e00113df116bb8ee36325dc5899b400da548b56e0fc2ec8ebd956b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3ab248170c3e4249b1a92534d8f8cb930da18a121812b2e3278ec8c2d9294485
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62306153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aeea0c5057a2c9bd77f4eadcb14a93ebc261bda8c9514fcdb762a0d36cbe5fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 23:19:39 GMT
ADD file:11f2036244afbd13a8d3e9654c8d3f3c99ab9e95ef31da94eed913ef504d6402 in / 
# Tue, 18 Oct 2022 23:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:090d64299c33248904e88674db63d2249fd29a5edf13fb417725a29c0819b946`  
		Last Modified: Tue, 18 Oct 2022 23:20:40 GMT  
		Size: 62.3 MB (62306153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:045dc0239192ac57f1fdc0a9cbb7a439e304f5bf5889256df234b1f5b23e23f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9b86385f3bc215268006627fbd6c23ec51b18756ea5b4e068ae8900c16af9253
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515011060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27784d8c4b05aa4fbb3556fe55ae176abb2c16639f09575e40dd65f617d9cc57`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 23:19:39 GMT
ADD file:11f2036244afbd13a8d3e9654c8d3f3c99ab9e95ef31da94eed913ef504d6402 in / 
# Tue, 18 Oct 2022 23:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 23:20:02 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6ba2180923a2f0b8f246ae7be3845522efffb9448264973c7b5f811296052d2c.tar.gz"     && echo "61c3e2a1535708dda90f5aa3cc856487b4950505f5c23e2e157933ced6a29670  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:090d64299c33248904e88674db63d2249fd29a5edf13fb417725a29c0819b946`  
		Last Modified: Tue, 18 Oct 2022 23:20:40 GMT  
		Size: 62.3 MB (62306153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc7431b327c65a3885610990e3515567e38c205976f395c3964df42dd030c5`  
		Last Modified: Tue, 18 Oct 2022 23:21:09 GMT  
		Size: 452.7 MB (452704907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220907.3`

```console
$ docker pull amazonlinux@sha256:76029546e00113df116bb8ee36325dc5899b400da548b56e0fc2ec8ebd956b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220907.3` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3ab248170c3e4249b1a92534d8f8cb930da18a121812b2e3278ec8c2d9294485
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62306153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aeea0c5057a2c9bd77f4eadcb14a93ebc261bda8c9514fcdb762a0d36cbe5fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 23:19:39 GMT
ADD file:11f2036244afbd13a8d3e9654c8d3f3c99ab9e95ef31da94eed913ef504d6402 in / 
# Tue, 18 Oct 2022 23:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:090d64299c33248904e88674db63d2249fd29a5edf13fb417725a29c0819b946`  
		Last Modified: Tue, 18 Oct 2022 23:20:40 GMT  
		Size: 62.3 MB (62306153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220907.3-with-sources`

```console
$ docker pull amazonlinux@sha256:045dc0239192ac57f1fdc0a9cbb7a439e304f5bf5889256df234b1f5b23e23f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220907.3-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9b86385f3bc215268006627fbd6c23ec51b18756ea5b4e068ae8900c16af9253
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515011060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27784d8c4b05aa4fbb3556fe55ae176abb2c16639f09575e40dd65f617d9cc57`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 23:19:39 GMT
ADD file:11f2036244afbd13a8d3e9654c8d3f3c99ab9e95ef31da94eed913ef504d6402 in / 
# Tue, 18 Oct 2022 23:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 23:20:02 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-6ba2180923a2f0b8f246ae7be3845522efffb9448264973c7b5f811296052d2c.tar.gz"     && echo "61c3e2a1535708dda90f5aa3cc856487b4950505f5c23e2e157933ced6a29670  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:090d64299c33248904e88674db63d2249fd29a5edf13fb417725a29c0819b946`  
		Last Modified: Tue, 18 Oct 2022 23:20:40 GMT  
		Size: 62.3 MB (62306153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affc7431b327c65a3885610990e3515567e38c205976f395c3964df42dd030c5`  
		Last Modified: Tue, 18 Oct 2022 23:21:09 GMT  
		Size: 452.7 MB (452704907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:3fb665f2087ec20639345185a7f2dfa36db149dce001bd5f388be02e0659e5a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:356a94b024b22e8f9b98a4f96065162e272983075668f2a4b7f5a77bac6957a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57654075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5983d2e603f74316b987b60a8d772258e5dcb2c50f4e6c8b66d7a3f155f3b817`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 06:50:24 GMT
ADD file:255cfef7726a0d303aef1490fb1cfcf29e287e0d8d240b878de9addd76ae894f in / 
# Wed, 26 Oct 2022 06:50:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:716ba0edb5da96c46c26a53c134cd740ead0345b7360bd6b9b467c7d00c8a677`  
		Last Modified: Sat, 22 Oct 2022 04:05:57 GMT  
		Size: 57.7 MB (57654075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4f9b0aadd51a2eecb4fa8b172af3c7d8e26d09e1a7787e5c2be17b9900f264b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56503263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9bb2305ccf4e86965736946e03d3c63821c4217b9c457dbd59ef57abe7eaef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:40 GMT
ADD file:8e97e9fb390fdbe0310f15a7de5dd86007e0d14993c44e64ee41db0d84824ff1 in / 
# Wed, 26 Oct 2022 15:27:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:903c8b1761ee036565aa58733a8a25f9b86a98e759ab3efe409019e4d4b0dea5`  
		Last Modified: Wed, 26 Oct 2022 15:28:59 GMT  
		Size: 56.5 MB (56503263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:1b6a3cf78359d45cff778c0b542bf66ec0c9fc3c1735d0d3a4f60ae0d8a54911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:eb03889b4ba3cedac439ce0d5c9f27234109f71356684cf4ceccb8d9b245b5a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.8 MB (387784962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20868dc236eb38a2f45fab9b54c56ea5f685204f68019e30fa40d04ec7381912`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 06:50:24 GMT
ADD file:255cfef7726a0d303aef1490fb1cfcf29e287e0d8d240b878de9addd76ae894f in / 
# Wed, 26 Oct 2022 06:50:24 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 06:50:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-14e16a3e28a8c27ff919b56d44ea297047f17e0eeadd435b2d71b68d50102537.tar.gz"     && echo "cee7a872aa60832489fa047b858cac4c9d5076a9a595d514fee06e816d406f80  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:716ba0edb5da96c46c26a53c134cd740ead0345b7360bd6b9b467c7d00c8a677`  
		Last Modified: Sat, 22 Oct 2022 04:05:57 GMT  
		Size: 57.7 MB (57654075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86aea60721dcdf4beeecb63a8df31330acdac43fe37466a09f951e571d1cee`  
		Last Modified: Wed, 26 Oct 2022 06:51:50 GMT  
		Size: 330.1 MB (330130887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:add79a7ef50521092c54edb7de96453991711647a6c92bde0878cc5636c1b872
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.6 MB (386634148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92662e39e0c8fda60f06351346cb7d9246b3202be7f9f14ed4797d80dbb76e8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:40 GMT
ADD file:8e97e9fb390fdbe0310f15a7de5dd86007e0d14993c44e64ee41db0d84824ff1 in / 
# Wed, 26 Oct 2022 15:27:41 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 15:27:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-14e16a3e28a8c27ff919b56d44ea297047f17e0eeadd435b2d71b68d50102537.tar.gz"     && echo "cee7a872aa60832489fa047b858cac4c9d5076a9a595d514fee06e816d406f80  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:903c8b1761ee036565aa58733a8a25f9b86a98e759ab3efe409019e4d4b0dea5`  
		Last Modified: Wed, 26 Oct 2022 15:28:59 GMT  
		Size: 56.5 MB (56503263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c84b504a5a9eb81ea0f91ff34bc0580d5b054ef32fee37e1c6d39b19f66c50`  
		Last Modified: Wed, 26 Oct 2022 15:29:22 GMT  
		Size: 330.1 MB (330130885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20221019.4`

```console
$ docker pull amazonlinux@sha256:3fb665f2087ec20639345185a7f2dfa36db149dce001bd5f388be02e0659e5a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20221019.4` - linux; amd64

```console
$ docker pull amazonlinux@sha256:356a94b024b22e8f9b98a4f96065162e272983075668f2a4b7f5a77bac6957a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57654075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5983d2e603f74316b987b60a8d772258e5dcb2c50f4e6c8b66d7a3f155f3b817`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 06:50:24 GMT
ADD file:255cfef7726a0d303aef1490fb1cfcf29e287e0d8d240b878de9addd76ae894f in / 
# Wed, 26 Oct 2022 06:50:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:716ba0edb5da96c46c26a53c134cd740ead0345b7360bd6b9b467c7d00c8a677`  
		Last Modified: Sat, 22 Oct 2022 04:05:57 GMT  
		Size: 57.7 MB (57654075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20221019.4` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4f9b0aadd51a2eecb4fa8b172af3c7d8e26d09e1a7787e5c2be17b9900f264b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56503263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9bb2305ccf4e86965736946e03d3c63821c4217b9c457dbd59ef57abe7eaef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:40 GMT
ADD file:8e97e9fb390fdbe0310f15a7de5dd86007e0d14993c44e64ee41db0d84824ff1 in / 
# Wed, 26 Oct 2022 15:27:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:903c8b1761ee036565aa58733a8a25f9b86a98e759ab3efe409019e4d4b0dea5`  
		Last Modified: Wed, 26 Oct 2022 15:28:59 GMT  
		Size: 56.5 MB (56503263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20221019.4-with-sources`

```console
$ docker pull amazonlinux@sha256:1b6a3cf78359d45cff778c0b542bf66ec0c9fc3c1735d0d3a4f60ae0d8a54911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20221019.4-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:eb03889b4ba3cedac439ce0d5c9f27234109f71356684cf4ceccb8d9b245b5a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.8 MB (387784962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20868dc236eb38a2f45fab9b54c56ea5f685204f68019e30fa40d04ec7381912`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 06:50:24 GMT
ADD file:255cfef7726a0d303aef1490fb1cfcf29e287e0d8d240b878de9addd76ae894f in / 
# Wed, 26 Oct 2022 06:50:24 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 06:50:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-14e16a3e28a8c27ff919b56d44ea297047f17e0eeadd435b2d71b68d50102537.tar.gz"     && echo "cee7a872aa60832489fa047b858cac4c9d5076a9a595d514fee06e816d406f80  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:716ba0edb5da96c46c26a53c134cd740ead0345b7360bd6b9b467c7d00c8a677`  
		Last Modified: Sat, 22 Oct 2022 04:05:57 GMT  
		Size: 57.7 MB (57654075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86aea60721dcdf4beeecb63a8df31330acdac43fe37466a09f951e571d1cee`  
		Last Modified: Wed, 26 Oct 2022 06:51:50 GMT  
		Size: 330.1 MB (330130887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20221019.4-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:add79a7ef50521092c54edb7de96453991711647a6c92bde0878cc5636c1b872
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.6 MB (386634148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92662e39e0c8fda60f06351346cb7d9246b3202be7f9f14ed4797d80dbb76e8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:40 GMT
ADD file:8e97e9fb390fdbe0310f15a7de5dd86007e0d14993c44e64ee41db0d84824ff1 in / 
# Wed, 26 Oct 2022 15:27:41 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 15:27:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-14e16a3e28a8c27ff919b56d44ea297047f17e0eeadd435b2d71b68d50102537.tar.gz"     && echo "cee7a872aa60832489fa047b858cac4c9d5076a9a595d514fee06e816d406f80  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:903c8b1761ee036565aa58733a8a25f9b86a98e759ab3efe409019e4d4b0dea5`  
		Last Modified: Wed, 26 Oct 2022 15:28:59 GMT  
		Size: 56.5 MB (56503263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c84b504a5a9eb81ea0f91ff34bc0580d5b054ef32fee37e1c6d39b19f66c50`  
		Last Modified: Wed, 26 Oct 2022 15:29:22 GMT  
		Size: 330.1 MB (330130885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:3fb665f2087ec20639345185a7f2dfa36db149dce001bd5f388be02e0659e5a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:356a94b024b22e8f9b98a4f96065162e272983075668f2a4b7f5a77bac6957a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57654075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5983d2e603f74316b987b60a8d772258e5dcb2c50f4e6c8b66d7a3f155f3b817`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 06:50:24 GMT
ADD file:255cfef7726a0d303aef1490fb1cfcf29e287e0d8d240b878de9addd76ae894f in / 
# Wed, 26 Oct 2022 06:50:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:716ba0edb5da96c46c26a53c134cd740ead0345b7360bd6b9b467c7d00c8a677`  
		Last Modified: Sat, 22 Oct 2022 04:05:57 GMT  
		Size: 57.7 MB (57654075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4f9b0aadd51a2eecb4fa8b172af3c7d8e26d09e1a7787e5c2be17b9900f264b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56503263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9bb2305ccf4e86965736946e03d3c63821c4217b9c457dbd59ef57abe7eaef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:40 GMT
ADD file:8e97e9fb390fdbe0310f15a7de5dd86007e0d14993c44e64ee41db0d84824ff1 in / 
# Wed, 26 Oct 2022 15:27:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:903c8b1761ee036565aa58733a8a25f9b86a98e759ab3efe409019e4d4b0dea5`  
		Last Modified: Wed, 26 Oct 2022 15:28:59 GMT  
		Size: 56.5 MB (56503263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:1b6a3cf78359d45cff778c0b542bf66ec0c9fc3c1735d0d3a4f60ae0d8a54911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:eb03889b4ba3cedac439ce0d5c9f27234109f71356684cf4ceccb8d9b245b5a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.8 MB (387784962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20868dc236eb38a2f45fab9b54c56ea5f685204f68019e30fa40d04ec7381912`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 06:50:24 GMT
ADD file:255cfef7726a0d303aef1490fb1cfcf29e287e0d8d240b878de9addd76ae894f in / 
# Wed, 26 Oct 2022 06:50:24 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 06:50:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-14e16a3e28a8c27ff919b56d44ea297047f17e0eeadd435b2d71b68d50102537.tar.gz"     && echo "cee7a872aa60832489fa047b858cac4c9d5076a9a595d514fee06e816d406f80  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:716ba0edb5da96c46c26a53c134cd740ead0345b7360bd6b9b467c7d00c8a677`  
		Last Modified: Sat, 22 Oct 2022 04:05:57 GMT  
		Size: 57.7 MB (57654075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86aea60721dcdf4beeecb63a8df31330acdac43fe37466a09f951e571d1cee`  
		Last Modified: Wed, 26 Oct 2022 06:51:50 GMT  
		Size: 330.1 MB (330130887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:add79a7ef50521092c54edb7de96453991711647a6c92bde0878cc5636c1b872
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.6 MB (386634148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92662e39e0c8fda60f06351346cb7d9246b3202be7f9f14ed4797d80dbb76e8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:40 GMT
ADD file:8e97e9fb390fdbe0310f15a7de5dd86007e0d14993c44e64ee41db0d84824ff1 in / 
# Wed, 26 Oct 2022 15:27:41 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 15:27:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-14e16a3e28a8c27ff919b56d44ea297047f17e0eeadd435b2d71b68d50102537.tar.gz"     && echo "cee7a872aa60832489fa047b858cac4c9d5076a9a595d514fee06e816d406f80  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:903c8b1761ee036565aa58733a8a25f9b86a98e759ab3efe409019e4d4b0dea5`  
		Last Modified: Wed, 26 Oct 2022 15:28:59 GMT  
		Size: 56.5 MB (56503263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c84b504a5a9eb81ea0f91ff34bc0580d5b054ef32fee37e1c6d39b19f66c50`  
		Last Modified: Wed, 26 Oct 2022 15:29:22 GMT  
		Size: 330.1 MB (330130885 bytes)  
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
