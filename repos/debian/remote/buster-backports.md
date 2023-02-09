## `debian:buster-backports`

```console
$ docker pull debian@sha256:374fbf30c7ce3581315976b7eb509c6bf6836338b265653e239e05896e5e2d2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:cd6c7898584bcd1919f7caf7610f9ff4f1da43fbfdd48800553e0949b6d04f0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50449836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e0f617d2b2c3a086af31e9626f3a10859931f595292b840519b39524406728`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:33 GMT
ADD file:dc52371b5f4608e5887e8c657ff951d1895e0047960f44b153c4a55ebf1726d5 in / 
# Thu, 09 Feb 2023 03:20:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:20:37 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b2404786f3febb4866f85b0c8f52b0b0b94dfdb6543e94cd65f961c68f325ff7`  
		Last Modified: Thu, 09 Feb 2023 03:25:32 GMT  
		Size: 50.4 MB (50449613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d81e9f907a1a2a9dbdef7fb7399467f800ccb7b2f6a2e54758d5c3ee517fee8`  
		Last Modified: Thu, 09 Feb 2023 03:25:44 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:83e731de3ddce924a1142f626ca7e4fa54228d3a61a19cdd09fffb35ec7f4874
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c67192bb0acfb0fa84784de6d4d09356c2395c07a5ba5431d5d3287f12912b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:50 GMT
ADD file:afaf1103e4ec74dcbbf13ec6a8049b78c15a909b8713dce5796a5ef6d7d5cbd4 in / 
# Sat, 04 Feb 2023 09:59:50 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 09:59:56 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6dcab737b693be9e498f0363e4109adad2721ce23274f5579d19c70a85bd0dd6`  
		Last Modified: Sat, 04 Feb 2023 10:06:48 GMT  
		Size: 45.9 MB (45915803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabc0f31b05ed5895e1440263bd8c57b30120a83ff7016c7ef930fa4afe1b4a`  
		Last Modified: Sat, 04 Feb 2023 10:07:06 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:12be25ce06122f16ec59c850de03cd95be73b20292851d94777075a7f4374098
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49239342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7008e9e33af669b8d9186d2aa6f945893e7d5a9265d608d0b387dac1b701e55`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:48 GMT
ADD file:fba5b8ea423b27a3182ca7344a0d2365acc105b05b21a0da48675799058af042 in / 
# Thu, 09 Feb 2023 03:58:49 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:58:52 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4b9dcf1a413259e77edbbd27343105dd36806b4cafcd111a22643d0f4b9a619f`  
		Last Modified: Thu, 09 Feb 2023 04:02:52 GMT  
		Size: 49.2 MB (49239119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3999ac58f2a23d8ef78aa6964cbfc1f5a69bd1cb1a8ce5f10b1c628fd4eaaf`  
		Last Modified: Thu, 09 Feb 2023 04:03:05 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:fdbc9883a625afee0c4183acd4c68065b18e67e70e2f20ff7e59a1839197f656
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ba93fcbdc2b53ec8cce9e00355c7c3b0ec3e525c42edd09bd754845f2f01c5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:33 GMT
ADD file:23aa007679cd84321e9278c9f6261256b1734b2e27727d84ecd3e3418e6b8dff in / 
# Sat, 04 Feb 2023 07:49:34 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:49:39 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:18e547e593209084f2c8150bc5b70229a02a902a855c32fb560765e6a40891a2`  
		Last Modified: Sat, 04 Feb 2023 07:55:26 GMT  
		Size: 51.2 MB (51207661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e04e4292b3c422cb10c9dc48ad222f7204c92d9581ebef91f4fe19be535c9e`  
		Last Modified: Sat, 04 Feb 2023 07:55:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
