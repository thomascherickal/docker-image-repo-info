## `debian:rc-buggy`

```console
$ docker pull debian@sha256:8350be575e3b2aa8ee21fa5766a29ccd83318768fa0841afa2f8b894bd2f6b8c
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:815a011d86e96d458601f5da9faffa9b9898cbcc2350fa8c64fd396b269c3f0d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55493476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04420ba08f80356b4d9dbea65a1bb24ea5ea3223fa156b5c5779f90e7ec8782b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:48 GMT
ADD file:7ab12da96bcf5f352bcecb8ee3269debf1ca1bd2d25aa9a7b66b1e4f84e07c3a in / 
# Fri, 03 Sep 2021 01:22:49 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:24:45 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f9ad9a9c210fa67e2eb0faace583b349a4623b682daec47e2b4c65c33ac9a92f`  
		Last Modified: Fri, 03 Sep 2021 01:30:17 GMT  
		Size: 55.5 MB (55493249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c568c6608b9a4ada48f98c4fb273d53b58f2979f960b4ade731dc8575640cf4f`  
		Last Modified: Fri, 03 Sep 2021 01:33:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:508923bd606cdac6e82b63b7d5dc154751cf01a837c87c924af4b86acb987098
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52980296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f48ab7519a99019e0dca92c8f751b0bb816aea6a6de3e8ec9fe39d61c138606e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:58:01 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afd540579db4a1768c8103d1cb013d6e9743b009387cb612f444a6c3c0face5`  
		Last Modified: Fri, 03 Sep 2021 01:17:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:14ef5c59e4d4f92d15f70c16294bcf8dd9640d18ef7ad37179700dc4e19c4336
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50638192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea984d91346240a84ae48ad524bc4536e1b0f0f5d13d4d044aac26c47fa42df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:03:00 GMT
ADD file:78431ef521d2864441ad8fd6f5238d8c49ff519c7f8510394048cc042f270288 in / 
# Fri, 03 Sep 2021 01:03:01 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:07:29 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:669a70f2eaf280942d3e643fd270beb3d6f313daba0d40fa8f3a72810a1e9bbb`  
		Last Modified: Fri, 03 Sep 2021 01:19:37 GMT  
		Size: 50.6 MB (50637968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33277f426372541d706ecb82581a45d91abe061dc993337ebc95442629226`  
		Last Modified: Fri, 03 Sep 2021 01:25:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:49c95a5f0ab74474f3fb2e983cc3fcc9c3760be03bcbe5413963cdd43334036c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54529345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c7d022e177f28feb76bbf3c7f8f218268601493e84a7caa0d3842935a5b983`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:54 GMT
ADD file:e9cb8fff7ac62f9bc8a4ccbc3960693736104975b5c3ffc855a1b6dea13b4c10 in / 
# Fri, 03 Sep 2021 00:41:54 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:43:42 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2cf0882b72727438ab6f57aa6a77711053bee00d53c08f527d6fc8e582fcdb3f`  
		Last Modified: Fri, 03 Sep 2021 00:51:39 GMT  
		Size: 54.5 MB (54529119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf1158bd858c02a980e161fa61f7f8d21534492541ff1c09b3058049e2c76d7`  
		Last Modified: Fri, 03 Sep 2021 00:55:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:8fe0c7566e340dbccf6bbe75feacc3ef11b65db3b0f66500e1b114e11ed12a8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56525492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a93f4bc296dff802ec9e01085fe1435d50c08a228717fa00a34a1d2f1bcc9c32`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:36 GMT
ADD file:64515d15f0b2fac0544e320a88716de6bf306c10f7e9400a945fca420a730843 in / 
# Fri, 03 Sep 2021 00:41:37 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:43:54 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:965ebee0ec76f6f76a0d14e40b7923292e9028532546ec1a748a8fed8267c897`  
		Last Modified: Fri, 03 Sep 2021 00:51:22 GMT  
		Size: 56.5 MB (56525268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1650096c87520af1d519d414681f0fed9d10ea3925c2fd75334c84b13d2eee7f`  
		Last Modified: Fri, 03 Sep 2021 00:55:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:6c2ab170705e4f8c9859dc0884927541d0d677118bd7e75deafee7fdef76b7d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54135231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e8b12234e65174d9514648cba937ebcb4d9d7b3f8d29fc5a7446a5563e2f012`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:14:59 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec6d79747c53c9c36b0b8a5265b1bfe515f43756465b52eb6f87ded8b88741`  
		Last Modified: Fri, 03 Sep 2021 01:26:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:bf02f52b0cef37c5dd890d9caa2cc859d5e0c197806b43db1ebe6ebdb26a22a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59534299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49da3929aacc93abff8f77a8ee15827c1aaa987292cf8781aacb8f76e67addfe`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:30:39 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c055d4d6c20555e40f6f325ce64682784d28fded349f4a0863224dd64d114e`  
		Last Modified: Fri, 03 Sep 2021 01:50:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:1bef80d72c51f24aaa1d1b3e5b5dd8aa1a52a97efe4ae744797384019b00bb88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53772378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b99bf22b92cdfb968eac2a1af99f053d19d4cd1989994757189dc7637a4a8fb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:46:03 GMT
ADD file:4dec873e9e3022f644e228769ed26be34f63fb2d9b0ddc10816af8c9eaa11a15 in / 
# Fri, 03 Sep 2021 00:46:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:49:25 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2c1522cfd5f84804048a7cb823dfa679d77781943db2c6e71d872921d6d7542e`  
		Last Modified: Fri, 03 Sep 2021 00:54:32 GMT  
		Size: 53.8 MB (53772150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edcbad45f190d09dcab6075b0d89e34423572b213df7ac337fd7e03c1f184f5`  
		Last Modified: Fri, 03 Sep 2021 00:56:42 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
