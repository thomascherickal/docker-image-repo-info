## `debian:experimental-20230411`

```console
$ docker pull debian@sha256:ee7ec1c012d1a21857270172d2299ee143ea5192bf4e476edd7628bdf1b635fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; arm variant v7
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental-20230411` - linux; arm variant v7

```console
$ docker pull debian@sha256:457923685976ee8c6aaf6bc51b5eba2513f7b372cf1813dfc66f7a2d42d3f5cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45890459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ef959bc2bb82aa080821852f23fc9669fd3daa05a2aa8c61afe1b7eca65041`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:29 GMT
ADD file:a85f9bd069b317fe04f7b0e5e2a6e54a4a94ed304e2487154c520f160f81634f in / 
# Wed, 12 Apr 2023 00:01:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:01:39 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:54d799b49c2235300dac823b010337407851814391945952bc9cbe2adfc39d3c`  
		Last Modified: Wed, 12 Apr 2023 00:06:16 GMT  
		Size: 45.9 MB (45890238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f266b9874326d8744696ecb20f43c6a235ce3e66b7ddfb6a034f15e3737e4f`  
		Last Modified: Wed, 12 Apr 2023 00:06:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230411` - linux; mips64le

```console
$ docker pull debian@sha256:21f20e067b8c031a8411cefeb6dbaee8ebc2ee5bef352928e7404e0afb99907a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49296474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c57b62d7b0bc81496cd6c4f650b7976e091f9170838b072b848d4ead104337c3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:13:36 GMT
ADD file:7175a1b08b8243bc539cc1f758d85ccbe24afbc3df6a1f629c7a43839aee5f62 in / 
# Wed, 12 Apr 2023 00:13:41 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:14:15 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:589b4c3c9d360e937d4513f3ec8af4982019090cf0f68fb06e1e275c06591a76`  
		Last Modified: Wed, 12 Apr 2023 00:21:40 GMT  
		Size: 49.3 MB (49296251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e8aaafc25e00fed4f728c0664478dccdcf9f43ed1708ea8ccbe0fbaed2a1bb`  
		Last Modified: Wed, 12 Apr 2023 00:22:19 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230411` - linux; ppc64le

```console
$ docker pull debian@sha256:1ee69d64a8be19f5bd1e06a74ffc9cf2726fbd4a286c70863f13a57e58b18b88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53291933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c76d7554eabcbe88b5cedc818303dc922fb264b836768deef356515d8d2da76`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:10:38 GMT
ADD file:930aae2ab6be5d8295a31bf5dd91eee5ee4fa92a08b6159f55cdc6d3bd182e67 in / 
# Wed, 12 Apr 2023 00:10:41 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:10:59 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4e67fd8b6f31e9a06c3401edfed958df31a0ae78d0692baa41a3d87074423b51`  
		Last Modified: Wed, 12 Apr 2023 00:15:52 GMT  
		Size: 53.3 MB (53291712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27112dd79fe0a748333ffc777c2b7353783f06d8bae54c98d2cfa0f7eb90dd40`  
		Last Modified: Wed, 12 Apr 2023 00:16:18 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230411` - linux; riscv64

```console
$ docker pull debian@sha256:848f36bcdc59386757ea640d87b9543b0b0e6974b24753e43c9d62a92cfe49a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45495174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:003a05cc9ec6850682d28a3624bb3de33c33df72a821c873287809c8e36a4c8c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:10:30 GMT
ADD file:f48330c22d0ecd502b8b46026eeef4081864a8a585160caae93e5700a6524a58 in / 
# Wed, 12 Apr 2023 00:10:32 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:11:18 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1b037784414a5f8d993a1f29169b41dbec924bf914e4e324fdd3209ce4445a32`  
		Last Modified: Wed, 12 Apr 2023 00:13:57 GMT  
		Size: 45.5 MB (45494945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91927993230d3dd4786ac01888e74b7a400d90f94093954b120def27101a238d`  
		Last Modified: Wed, 12 Apr 2023 00:14:43 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230411` - linux; s390x

```console
$ docker pull debian@sha256:9bb2165075db3a6509a9447f86beafeac8f7ba75202b764da22b505ec16b170a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47665290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a0a7b534b879a5d04f757626e6f6acf5a4dad5380f6c29124d4cce3940a4ccb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:03:33 GMT
ADD file:9280167c5f0a6008baa6e9d84a780823b1cf741a9935a60531fb30279a421a97 in / 
# Wed, 12 Apr 2023 00:03:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:03:54 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:967d5de3f09581dfdc9be32037966130e96015074ba7d995ffb521bcb496aedb`  
		Last Modified: Wed, 12 Apr 2023 00:06:36 GMT  
		Size: 47.7 MB (47665070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d61ec497f5f76e5e6a2d2a829e93a2e43b9ad2cbc9586ab0729461604adb3c`  
		Last Modified: Wed, 12 Apr 2023 00:06:49 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
