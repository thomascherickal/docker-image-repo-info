## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:ac3637b886baf24b1fd2b8699408aee21e9be0747aa8af97ab55fcb24697e659
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:fcfb141972e46548e9e1242a7c45c5cb19015b198d45e288e26fdec064bd60a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50436108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9c3b27634846a81b3dd7fa89796002bf5bcf289468eae3228f70ba5fcb7b51`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:23 GMT
ADD file:25c6af0cf8f175682054f5614095359181f717b97a13115299c747a1acfc6e78 in / 
# Fri, 03 Sep 2021 01:22:23 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:22:29 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:67899ba80f32cae9c5a2a1ff823dd71bb6885b253229e597cbcae29b36fb45e0`  
		Last Modified: Fri, 03 Sep 2021 01:29:29 GMT  
		Size: 50.4 MB (50435884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a40ffd8618f06297f6896b5426d7a8362260534a9e5d6dec821a05d00bd75e`  
		Last Modified: Fri, 03 Sep 2021 01:29:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:251e75eb88e7895e60808778cc7ef357035502e64c5ed82b9e3bce8942ff6ca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48154028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32bdfe1c4f99ae404fc7887ec9d7c38de79f31db9dba5958a918540724c26f8f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:52:46 GMT
ADD file:36cdcba9b88e084699a204bfa2d0f4cec055962b94a4360c41db5b15ebfcde01 in / 
# Fri, 03 Sep 2021 00:52:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:52:59 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e33b0ff4e89656be3954d22db72c6e49ad3039670739b8ec39ba0cb1c5fb9466`  
		Last Modified: Fri, 03 Sep 2021 01:09:16 GMT  
		Size: 48.2 MB (48153802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55703fea4ebc50cd25cffede1611abf646a97cf41c0317f46a69e725570852`  
		Last Modified: Fri, 03 Sep 2021 01:09:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:99f391502886301f61578614fa6dcaa6c069572782a880d5be144ff7e5eed1b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45917738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f173d1a975136aaa084de340f475c8aa38ba315a4078cbfc487112617fd2d5e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:02:03 GMT
ADD file:17995ec5935167f8cfb9f959ee5e14c9dd7f7e9671a65abe443b39988934dce3 in / 
# Fri, 03 Sep 2021 01:02:04 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:02:16 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4583284ddbf17c7cc8c8ad1fdfc30f52eeda1a4f6dc7644108c26362263af3cc`  
		Last Modified: Fri, 03 Sep 2021 01:18:24 GMT  
		Size: 45.9 MB (45917513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575de22dab8f7438143877309c351c5e95ef038f4848e14472caa1e96822d5c9`  
		Last Modified: Fri, 03 Sep 2021 01:18:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:9e2dc07476e94930b85f702b355578a51a02f2ec4c075fb07cc7a072568e397b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49222331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca58b107e926301ee2b1addec9659cce36781e983773bd6cf079d20a8ac55c34`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:30 GMT
ADD file:bd2f587c11f381138607533603c6012513a700b56b464d65189cb96550d45533 in / 
# Fri, 03 Sep 2021 00:41:31 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:41:37 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0f1c1ed3748f861b03424f8c90aa139436cef2978931e7e07823bdf46e1635a5`  
		Last Modified: Fri, 03 Sep 2021 00:50:55 GMT  
		Size: 49.2 MB (49222110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c7089ddf38e30f0aa372277d058125a338a6de132721a9bfc869ae822b40ca`  
		Last Modified: Fri, 03 Sep 2021 00:51:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:f220d307a6690023485cfe9957b6eb5b7c4110c9b787722cbcce60292bc70bec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a4b538467a5d48acdc84996735247434de30c9a61ccb58e2672622158305d4a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:07 GMT
ADD file:29e08bd5abf67e862792b22f78257915519cb0519b913e116db0254ec9897785 in / 
# Fri, 03 Sep 2021 00:41:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:41:13 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fc8b5543cb8abcef10221a0c8e128bcf826e018e6070d7d24db3c61964e15b53`  
		Last Modified: Fri, 03 Sep 2021 00:50:34 GMT  
		Size: 51.2 MB (51207223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fe1b03495ddba8707e27415bae33cc22b8a94b5980afc1f0158319429e5f7f`  
		Last Modified: Fri, 03 Sep 2021 00:50:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:637049b05671854ff622e4f40642eb415590f79796c46f9a4c9bfadc06abb231
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49080304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf836854d4fde3ce13cfa07208cce9578b2f105f72691ba9518ab92f9675771`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:11:14 GMT
ADD file:b3a0336c03cde91518be1189cdca3185276e9c9e965d5e123b766b8399bd3e1d in / 
# Fri, 03 Sep 2021 01:11:15 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:11:21 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:91339a4d49208e09b5b1324d90f5dc6104bb35ccb61135662b98533970c514f2`  
		Last Modified: Fri, 03 Sep 2021 01:20:36 GMT  
		Size: 49.1 MB (49080080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae91dc7b06123ad83c662741d20d8b890516ca85ed88ba4aa2c0432d3f0a3dc8`  
		Last Modified: Fri, 03 Sep 2021 01:20:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:44b40ab18a1b025c71b6b25c8daeba2a7ed29edce0657d436b1c6377ed754c94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54182888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c694c2b9723790899a70fb6d7866e97109b7a9393dd14f0267abdf2b94d62fc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:25:01 GMT
ADD file:0de8dbd369ea8a734934d859b2127ac2d170c7c67ed97b1969a240f3a20f0806 in / 
# Fri, 03 Sep 2021 01:25:14 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:25:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ec7b038dfffa75a312736217d90bbf467ce4af7129e08320361872aa43b27d4`  
		Last Modified: Fri, 03 Sep 2021 01:40:50 GMT  
		Size: 54.2 MB (54182660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d84750a2ec9d770a90f06a4971a6c6d26e845860843dad9ca2f724556fc877`  
		Last Modified: Fri, 03 Sep 2021 01:41:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:7b1371c66be74d0e5e1775f1a361df69c9a6dbb435fe39e1da235d0637298c0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49004334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dfca3a7c2cebb916ccee583bc5cb7899242f3427735887f9341989da8e7ed44`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:45:06 GMT
ADD file:12a3d9c18585c5348accfaa080a4e184f57580993e45e50da1191497d679d889 in / 
# Fri, 03 Sep 2021 00:45:14 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:45:23 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:87e71254eea4f95aa14fe4a86494020777f6f8433e36ef91c491dc7401501304`  
		Last Modified: Fri, 03 Sep 2021 00:53:59 GMT  
		Size: 49.0 MB (49004111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9907e2df7c2a7fb9d0b90d82175e9614899325f7a8b3b7abca0dc1b2e31ac555`  
		Last Modified: Fri, 03 Sep 2021 00:54:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
