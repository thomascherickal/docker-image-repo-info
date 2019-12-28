## `debian:rc-buggy`

```console
$ docker pull debian@sha256:567f7e79a5c7810a9290d2631bb8e5efbcac2b8e20fe0b95635bc838513dd3e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:b8d9b614790088fe10e1cd2bd7de2c93152d463d55d4e31879856bded022bb51
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51479837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6861ec49fad42db840fa4ad529e20f0f07db2e86f0b99a3cb60b0a9996a58fd9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:22:47 GMT
ADD file:68b1541306250f957e5f1035d80f5683c1ed22e73cf2f2b563adc52424897a09 in / 
# Sat, 28 Dec 2019 04:22:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:24:43 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d0b468739e287d7cd8fa8bcb34afb10216f12567d28caab345db8873c4246896`  
		Last Modified: Sat, 28 Dec 2019 04:27:19 GMT  
		Size: 51.5 MB (51479608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45140dd244d8de9fdd1ce279f01844e4dbaaa698a45adf002f14eac3f91d7c0`  
		Last Modified: Sat, 28 Dec 2019 04:29:39 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:228f8c3ff8ab8b811564a922d69b95d6fd9b02b201cf1a7009ddc186f60f7c84
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49263386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb99101ce81976958014694b77b0637ec0750410a13528586eff84a398b3635`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 12:16:29 GMT
ADD file:b33940de85ef3cf7d3fda96a84c087cf2748d092b2c6dc801a10dba97bb280da in / 
# Fri, 22 Nov 2019 12:16:32 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:20:18 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:add7c672a81c67254d62a1133cde0c17aee030ac3cc9e62b142561c039c20fae`  
		Last Modified: Fri, 22 Nov 2019 12:24:42 GMT  
		Size: 49.3 MB (49263157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951f46d04d86c760b2229e18ac520fea7f834ba46b5407875ff487cac5e2455f`  
		Last Modified: Fri, 22 Nov 2019 12:27:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:13bd9a8b0542c89a6dd79b6e3791b7a9c172ae19a7870192ae51fdf10ab226a9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47016075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7430232234771e6d521267f7289a641d8ef9cf837c8780f192e294e8e707599`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:25:58 GMT
ADD file:4bf78bfddc69aff1005ff137dbb0900252b387eb72db243381eb8668106c1077 in / 
# Fri, 22 Nov 2019 13:26:01 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 13:31:30 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c9c2507cf34749b60069708965e9265b59dd74f435cb2b28decd5de28599b56f`  
		Last Modified: Fri, 22 Nov 2019 13:35:33 GMT  
		Size: 47.0 MB (47015849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d4d9e5d86b241f182aed93835a5aa5c713b73267579c29539c0753b098eb47`  
		Last Modified: Fri, 22 Nov 2019 13:38:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:52cd5baf98d1afa4fb04d8fe8260cf2eb55dd57fc7bef897c67bdcd1d57e4ab0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50431344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c2495fa3c427c63637ed9983242172744a3cad869e5fd40990a948450c787f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:8932c68f3cf662412b086b3ca8b215a092fa5ea459074d42d359a9c778563152 in / 
# Sat, 28 Dec 2019 04:42:05 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:45:16 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:898762c0a5be611b2ded7eb33fffee89def5fd9c6161871b3f1f06e970b7739e`  
		Last Modified: Sat, 28 Dec 2019 04:47:51 GMT  
		Size: 50.4 MB (50431115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9745fcb903d5188e779a393a5569abe4528449b9748581d96bc3198b225265`  
		Last Modified: Sat, 28 Dec 2019 04:50:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:885402e351574d3a7b6990ae457999b8f14a40a95855de8da2bbe7ffbfceb709
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52610959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0840be6c025010de498e800eee12450eedd81a5aa65aca636c5c5a71f3e46ff2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:02 GMT
ADD file:028a6b956388b2cf033fb64213fca841fe5708f01d7143a9883bb44273bfb987 in / 
# Sat, 28 Dec 2019 04:41:02 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:43:05 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b389037d8e8619e17e0b7de53ac2f84439d0b5b064350f604942c26d3b2f2608`  
		Last Modified: Sat, 28 Dec 2019 04:46:15 GMT  
		Size: 52.6 MB (52610734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf483d4b4ab04214c9498eb8565540eb864d3ceb9e58379f4a5f7d365f777e3e`  
		Last Modified: Sat, 28 Dec 2019 04:48:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:3eac7b54e3bc9f3b650771baa6bda231976b29e65c0787c9e80f2d362f6a0f3a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55285208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbceafdd5884af4934dd8ad4af196bed2b34e35d3898a53b220afe04bf89c76d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:44 GMT
ADD file:d7ba1f92f51134645d0c28cccf74dc6cc9cff62c18d1e7ea24e9306b603cc4c6 in / 
# Sat, 28 Dec 2019 04:21:49 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:24:59 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a19f8e61b2d8b008c7115d66fcae892bce80e022931657219cecb2a15110c398`  
		Last Modified: Sat, 28 Dec 2019 04:29:56 GMT  
		Size: 55.3 MB (55284979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daefea6ef529872c79f58b2e841b934df523e5cea0eb6ea12bffb0aa6fc43b28`  
		Last Modified: Sat, 28 Dec 2019 04:36:13 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:6d4cb8ceade93a43d038bb64e90fa5aad2e3d82dcb51d5d0d7afe2523edfc41c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50131811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9371e3d7efae654f4a809b02e9b5d8a96d4c7a5421d9d36ab7cd9b3a3f8eb210`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:32 GMT
ADD file:ebe1df568622bb8e8e8e3b2318d11550389d84f3196d3ade9aaa9ecfdecd1028 in / 
# Sat, 28 Dec 2019 04:42:32 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:44:08 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7d0208a582df93acf7a81d059abd969865a1e647765a53c87e2123fb6b283a34`  
		Last Modified: Sat, 28 Dec 2019 04:45:42 GMT  
		Size: 50.1 MB (50131585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419bcbef09b36dc65a1330498acfbf407e4cfeb338ce6be779d5065d1094d4e3`  
		Last Modified: Sat, 28 Dec 2019 04:47:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
