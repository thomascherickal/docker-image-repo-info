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
-	[`amazonlinux:2022.0.20221012.0`](#amazonlinux20220202210120)
-	[`amazonlinux:2022.0.20221012.0-with-sources`](#amazonlinux20220202210120-with-sources)
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
$ docker pull amazonlinux@sha256:c6d435634683b58ab7ede834b90dd0d6d2bb55dfcc32b4f4e5175c50bb8c4a34
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
$ docker pull amazonlinux@sha256:82427411beee9ba40978c24eda7af42d5df1e076cff5d7fc5ffd3081814a07b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63919869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe239fc14dbf55c8cdaf7d7657a51c6290ed012b701f78baec576efad01fc73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:0f8885e4c7c5c5f70e056b3f454c8c57b3380a47cfdbeb1219cf28db5540086b
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
$ docker pull amazonlinux@sha256:9cb56adb55e362e1f0bc602fa374ee76f5c811694dd0fbb8115405ba485f9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487995276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69c9041ba9d726678c5b01f35d67267439fb39bd34ec3c1639468508c85fdf58`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
# Thu, 20 Oct 2022 23:39:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c50b200f4b88b34f76bfe2124998da6bcab84e615337b7fe7ddd2d8ac33114e`  
		Last Modified: Thu, 20 Oct 2022 23:41:19 GMT  
		Size: 424.1 MB (424075407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20221004.0`

```console
$ docker pull amazonlinux@sha256:c6d435634683b58ab7ede834b90dd0d6d2bb55dfcc32b4f4e5175c50bb8c4a34
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
$ docker pull amazonlinux@sha256:82427411beee9ba40978c24eda7af42d5df1e076cff5d7fc5ffd3081814a07b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63919869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe239fc14dbf55c8cdaf7d7657a51c6290ed012b701f78baec576efad01fc73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20221004.0-with-sources`

```console
$ docker pull amazonlinux@sha256:0f8885e4c7c5c5f70e056b3f454c8c57b3380a47cfdbeb1219cf28db5540086b
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
$ docker pull amazonlinux@sha256:9cb56adb55e362e1f0bc602fa374ee76f5c811694dd0fbb8115405ba485f9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487995276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69c9041ba9d726678c5b01f35d67267439fb39bd34ec3c1639468508c85fdf58`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
# Thu, 20 Oct 2022 23:39:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c50b200f4b88b34f76bfe2124998da6bcab84e615337b7fe7ddd2d8ac33114e`  
		Last Modified: Thu, 20 Oct 2022 23:41:19 GMT  
		Size: 424.1 MB (424075407 bytes)  
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
$ docker pull amazonlinux@sha256:9a8f402248e675582fc7a85b5571cfe930c4304350cebca34d4d7f4447f99319
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9be478e5302e819b22748b02cef9100fbe1d94fb2f686992bb1fe342e2f13617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff592f394353087fc68ed2ca76c2e93ef0530352e529cf4e24408fd19e50e0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f27d0cadf3b206e09b18623f6818f0956d878ab29fa00028c565e9f83b028eeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56481754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866f138fb6f3eef9cf1c6f7e3f9a6e139ed594eb1128b1599b0137b6d6e7ff5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:215c755f3dd70ebd198d5750e92052deb39debf83d3d365e95633bb01f1d9957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0595983489ba3b0fff0f7099f2b64174d8792d7863dc1a5a8eadaf779bc48e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.7 MB (386739246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5dbe9498109f5c7575eef6c4776278d4c5ea3c83f9ed55211873a5c38c1410`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:20:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f62047bb148ea45f7f34dc9e1bffbd74fa083fd7b6784e0dbed1685f6eb339`  
		Last Modified: Tue, 18 Oct 2022 00:21:06 GMT  
		Size: 329.1 MB (329081491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6b5dade9f05691b289fbbcd0e203d6e44ac7bc4c9a7bd8049e26e13e0a7b57c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385563209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77e861f60a2da3e2c3af5d4dcb8cd19a11a1862fa9b80ddccb0c168e8e3ec9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:40:04 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f3324e83ad5f6d382027fcf8d3c3b31785ddb076e0ccee7669e38742e29ce2`  
		Last Modified: Tue, 18 Oct 2022 00:41:16 GMT  
		Size: 329.1 MB (329081455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20221012.0`

```console
$ docker pull amazonlinux@sha256:9a8f402248e675582fc7a85b5571cfe930c4304350cebca34d4d7f4447f99319
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20221012.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9be478e5302e819b22748b02cef9100fbe1d94fb2f686992bb1fe342e2f13617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff592f394353087fc68ed2ca76c2e93ef0530352e529cf4e24408fd19e50e0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20221012.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f27d0cadf3b206e09b18623f6818f0956d878ab29fa00028c565e9f83b028eeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56481754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866f138fb6f3eef9cf1c6f7e3f9a6e139ed594eb1128b1599b0137b6d6e7ff5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20221012.0-with-sources`

```console
$ docker pull amazonlinux@sha256:215c755f3dd70ebd198d5750e92052deb39debf83d3d365e95633bb01f1d9957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20221012.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0595983489ba3b0fff0f7099f2b64174d8792d7863dc1a5a8eadaf779bc48e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.7 MB (386739246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5dbe9498109f5c7575eef6c4776278d4c5ea3c83f9ed55211873a5c38c1410`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:20:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f62047bb148ea45f7f34dc9e1bffbd74fa083fd7b6784e0dbed1685f6eb339`  
		Last Modified: Tue, 18 Oct 2022 00:21:06 GMT  
		Size: 329.1 MB (329081491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20221012.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6b5dade9f05691b289fbbcd0e203d6e44ac7bc4c9a7bd8049e26e13e0a7b57c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385563209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77e861f60a2da3e2c3af5d4dcb8cd19a11a1862fa9b80ddccb0c168e8e3ec9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:40:04 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f3324e83ad5f6d382027fcf8d3c3b31785ddb076e0ccee7669e38742e29ce2`  
		Last Modified: Tue, 18 Oct 2022 00:41:16 GMT  
		Size: 329.1 MB (329081455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:9a8f402248e675582fc7a85b5571cfe930c4304350cebca34d4d7f4447f99319
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9be478e5302e819b22748b02cef9100fbe1d94fb2f686992bb1fe342e2f13617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff592f394353087fc68ed2ca76c2e93ef0530352e529cf4e24408fd19e50e0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f27d0cadf3b206e09b18623f6818f0956d878ab29fa00028c565e9f83b028eeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56481754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866f138fb6f3eef9cf1c6f7e3f9a6e139ed594eb1128b1599b0137b6d6e7ff5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:215c755f3dd70ebd198d5750e92052deb39debf83d3d365e95633bb01f1d9957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0595983489ba3b0fff0f7099f2b64174d8792d7863dc1a5a8eadaf779bc48e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.7 MB (386739246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5dbe9498109f5c7575eef6c4776278d4c5ea3c83f9ed55211873a5c38c1410`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:20:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f62047bb148ea45f7f34dc9e1bffbd74fa083fd7b6784e0dbed1685f6eb339`  
		Last Modified: Tue, 18 Oct 2022 00:21:06 GMT  
		Size: 329.1 MB (329081491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6b5dade9f05691b289fbbcd0e203d6e44ac7bc4c9a7bd8049e26e13e0a7b57c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385563209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77e861f60a2da3e2c3af5d4dcb8cd19a11a1862fa9b80ddccb0c168e8e3ec9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:40:04 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f3324e83ad5f6d382027fcf8d3c3b31785ddb076e0ccee7669e38742e29ce2`  
		Last Modified: Tue, 18 Oct 2022 00:41:16 GMT  
		Size: 329.1 MB (329081455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:c6d435634683b58ab7ede834b90dd0d6d2bb55dfcc32b4f4e5175c50bb8c4a34
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
$ docker pull amazonlinux@sha256:82427411beee9ba40978c24eda7af42d5df1e076cff5d7fc5ffd3081814a07b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63919869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe239fc14dbf55c8cdaf7d7657a51c6290ed012b701f78baec576efad01fc73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:0f8885e4c7c5c5f70e056b3f454c8c57b3380a47cfdbeb1219cf28db5540086b
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
$ docker pull amazonlinux@sha256:9cb56adb55e362e1f0bc602fa374ee76f5c811694dd0fbb8115405ba485f9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487995276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69c9041ba9d726678c5b01f35d67267439fb39bd34ec3c1639468508c85fdf58`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
# Thu, 20 Oct 2022 23:39:58 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5739eed8c30abe39025fd3b2efc192206cf6c30a9ed1c856112143b6d7324455.tar.gz"     && echo "b2bcb16e488395c3f073ae7cf2cd2a3e979e50c0448777aadc746bc60348fc92  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c50b200f4b88b34f76bfe2124998da6bcab84e615337b7fe7ddd2d8ac33114e`  
		Last Modified: Thu, 20 Oct 2022 23:41:19 GMT  
		Size: 424.1 MB (424075407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
