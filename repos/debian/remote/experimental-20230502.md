## `debian:experimental-20230502`

```console
$ docker pull debian@sha256:41565377297ac145a7677812315dea43f629e7c65c940d55dd2bdd65bb3cf69d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386
	-	linux; mips64le
	-	linux; riscv64

### `debian:experimental-20230502` - linux; amd64

```console
$ docker pull debian@sha256:dde1617d7748bb57ba85a784bf30ba18879bbb19716af321fb0da1f1999638aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49299496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992fbf71860210a94838145a5d1647dbc879b30ae0b92daf39fd8eb758ae7f50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:48:33 GMT
ADD file:3bb0dbe1e0e6f100e1b1bf234d8abb124cb76a74c0a6534b96944aae00f2d783 in / 
# Tue, 02 May 2023 23:48:33 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:48:43 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b09d7a954016db203b7b9a15bce1153fb2a053c8ceeb27b62838c6a42b01e46e`  
		Last Modified: Tue, 02 May 2023 23:53:24 GMT  
		Size: 49.3 MB (49299275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c05a75dcc93de27a408b593d23b740952d152e3d644127ad318762a50f877e`  
		Last Modified: Tue, 02 May 2023 23:53:43 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230502` - linux; arm variant v5

```console
$ docker pull debian@sha256:3ec7e8d03d0b24136e45f16749d8e235bf15a53f31933b235167d4a787b5c68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47167286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97b434224c2e1b20ddc7accaa6b3353325c2f0a71b144f0b8014381fe091ee1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 22:49:42 GMT
ADD file:740dbf70289faed5b254bb33009aaddef87ef73abcfdc2441b61e0be62ac6d62 in / 
# Tue, 02 May 2023 22:49:42 GMT
CMD ["bash"]
# Tue, 02 May 2023 22:49:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c7b5fff53169be147228f50722828c1946b9253a79b37d14d755411593e715be`  
		Last Modified: Tue, 02 May 2023 22:53:28 GMT  
		Size: 47.2 MB (47167066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eade863a9332ac1f6ffe4dbd68aaf23ffd777b9c81619aeeccc0bf1aa40899e`  
		Last Modified: Tue, 02 May 2023 22:53:49 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230502` - linux; arm variant v7

```console
$ docker pull debian@sha256:1e29f5c8bf7272ff3a2cf41b0c5a6073a8989dc50708c4a6d5529b8fafa1c329
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44988301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f55497438ad2029200afad5cc89b70b82edef294e307f50ab16aa8a116abf6f0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:49:39 GMT
ADD file:32753ebe1bca84d98359b94076aecbac1b5009dbe8880e44b4f3ab811f285cfa in / 
# Tue, 02 May 2023 23:49:40 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:49:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1beaeabfc30425aef4331e1b03cb028a5a9571ce069e575ffe55571116d06bae`  
		Last Modified: Tue, 02 May 2023 23:54:44 GMT  
		Size: 45.0 MB (44988080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27c4469e65360ca8ea4f0d899ac1bcc4f28a330fe24210a715bd0a1f339c559`  
		Last Modified: Tue, 02 May 2023 23:55:06 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230502` - linux; 386

```console
$ docker pull debian@sha256:371ef1177f3f926033faaf5e0ef262cbf30a291ebe4e2efea17e4071d1094e01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50321998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392678835412005feb7257a5b7758bb1ded2fdf1b610bd585d8d4dc65ca50b50`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:03:13 GMT
ADD file:573ff628a65fa16a69bbc50413058747249b5b5874755985f981664678fcaaca in / 
# Wed, 03 May 2023 00:03:14 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:03:27 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:74c7d60e968ebc8c7e187d99ff063349554f2e3c69866ac4897d2d4f2c7ff26e`  
		Last Modified: Wed, 03 May 2023 00:08:44 GMT  
		Size: 50.3 MB (50321777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51d59dc39163bdab3318d74f51fbff67816f67def403fcc08334d640c279684`  
		Last Modified: Wed, 03 May 2023 00:09:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230502` - linux; mips64le

```console
$ docker pull debian@sha256:6691a30206d8af0061a1e30fcb3fe172024ad5b6d58a7d02b1e214d3d5c34553
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49301655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5612453c73a88f32734de438592cbb9257d4b80baf15075844255e8f2e441509`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:54:16 GMT
ADD file:5acf41935c7e4664ad9eaffb8eb6ff951f25e96188c7bb68c05b3beb4a05ecfa in / 
# Tue, 02 May 2023 23:54:21 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:55:07 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0f41ec9c841e5471c15b435f5869be0c4ddab2c10b732664d56c272673169ad2`  
		Last Modified: Wed, 03 May 2023 00:02:28 GMT  
		Size: 49.3 MB (49301431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599a125a54fcfe85549f7fe92ec5b299bd3ae7d296e67bea9051dbb9f99ec94a`  
		Last Modified: Wed, 03 May 2023 00:03:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230502` - linux; riscv64

```console
$ docker pull debian@sha256:9e6857cdbc35d18a1d079fb33fb05af3b7151f8b407e11139abee56a963d0833
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45510312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea683121a36ab714a62f0510e95aaafb08bea31fff3214005a832dc1f8fef968`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:30:42 GMT
ADD file:aec12b014e0d6fdd7f6cef74c98d05dc928194f272d810f72a5d101461dd448f in / 
# Tue, 02 May 2023 23:30:44 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:31:30 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:10ecef60835156e81af0a582263a6c0d66b80ef97202eae73cdd1b1265c7237b`  
		Last Modified: Tue, 02 May 2023 23:34:04 GMT  
		Size: 45.5 MB (45510083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e62b5d507e148e33139c193e57b2ea3f5aec931117139f8a7832490b98e2fe`  
		Last Modified: Tue, 02 May 2023 23:34:51 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
