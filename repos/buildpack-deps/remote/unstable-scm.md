## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:20d37c1005ae07c16a77312fa565ac3990399a169d5feac9e5368d43845087eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0abecfd3831c9b69c830ddadefd33d2ab68555ce081e9eb05c0cd44c2bd0b153
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127514561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3557e30291bd8748d13ae0a1df0419cd78a45eddb9d3e6f26d3ab66dcfe91cb6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:53:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b8f6b86e3a84210feef982a4953fcc1b15003e51b2fb7b861ae18f18e914f`  
		Last Modified: Tue, 28 Sep 2021 02:00:14 GMT  
		Size: 5.2 MB (5181002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e6a19825e33b3ebf505b0ae79fe6cf49091e693c4d8971abde683746f445`  
		Last Modified: Tue, 28 Sep 2021 02:00:15 GMT  
		Size: 10.9 MB (10900815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8600ac737a89c73eb8b73b618e244774719a3cc4caaa7325dbf6d6e04706ed`  
		Last Modified: Tue, 28 Sep 2021 02:00:34 GMT  
		Size: 55.7 MB (55730660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4cd97ee516ec215abbd5b3ac462930d5ce96d603e843d9e3c16f2f89b92fa7cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122339119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5cd7b304c5341441e3c2c40eeb8cb460e041906d3883be6d82bebca44295a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:54:15 GMT
ADD file:bcd1f002a3a38be54eed5da9d7a2e3822ecdf63ba82a59931124557d1f97007b in / 
# Tue, 28 Sep 2021 01:54:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:57:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4bd09bbbe96b85664474243c833d73be517c92e7172b8d740101438ee21d5561`  
		Last Modified: Tue, 28 Sep 2021 02:11:21 GMT  
		Size: 53.2 MB (53207754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70c595ca5d004271509bd463bf50b3dc2d385630237ea30f5e4936f414a9b7`  
		Last Modified: Tue, 28 Sep 2021 03:14:06 GMT  
		Size: 5.1 MB (5088778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e46f7c293bb67a0ab1c2bbce082b844bc145c04bb54e588fa2146980730af`  
		Last Modified: Tue, 28 Sep 2021 03:14:08 GMT  
		Size: 10.6 MB (10606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32e39f8615ccdb2930517a3daed84ef9540d8f34f9a6a2447c42b05dd7e6d93`  
		Last Modified: Tue, 28 Sep 2021 03:14:58 GMT  
		Size: 53.4 MB (53435709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7a0d1efa6e01ca27a3c8b6ce00256addbf9e6a87727403382b3bb85867f46245
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.4 MB (117390664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ca238d4f10dd5e6d87c27eca2dbd6a378f05ea84b11758f19a8a33cb2b27e0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:06:54 GMT
ADD file:d9a8e8032b2f681adb1be7e9dfacdf1838167068f97e052c3173223cb1d2c303 in / 
# Thu, 30 Sep 2021 18:06:55 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:39:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:40:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90a9a2564a394330c4b6320f33e007b55c6f40a9006b85fe17fa2ed9fe260cee`  
		Last Modified: Thu, 30 Sep 2021 18:23:58 GMT  
		Size: 50.8 MB (50822436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f06eb4253b6bc5ee446db688fa4b3052465b6890ef2f7157f1a345118360e`  
		Last Modified: Fri, 01 Oct 2021 05:58:43 GMT  
		Size: 4.9 MB (4946836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b50232f315931bda767b06cac42d2688e34c66a06877f32bc9bdb103575e50`  
		Last Modified: Fri, 01 Oct 2021 05:58:45 GMT  
		Size: 10.2 MB (10249907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6189d745298f970340832970521c77f9df62fa058d6a498469ecaac7cdd9e`  
		Last Modified: Fri, 01 Oct 2021 05:59:31 GMT  
		Size: 51.4 MB (51371485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3b8e35be88c4a91d8413351d8c621c65496a35142b7b0e4c7f97c9ade9a3f078
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126660892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51de9ff568cdc9fcc755ffef64b86ff3ac486276a65accf31b79039ae9812ff3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:20 GMT
ADD file:714781c9fce1c450e5f9cc5529167eaa33fdff089ab48a1dcac0a813d768be30 in / 
# Tue, 28 Sep 2021 01:42:20 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:18:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:18:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:19:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bd53cd90ab526d30a2e414c3951333db1b1b814fe009621017a07b5eea3cad0f`  
		Last Modified: Tue, 28 Sep 2021 01:51:10 GMT  
		Size: 54.7 MB (54725302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3945f16b6588acc2f82d3f0371dd15803436b26df556a96921d086d035a320cd`  
		Last Modified: Tue, 28 Sep 2021 02:27:09 GMT  
		Size: 5.2 MB (5169449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba2c20fe4248de05c9d215800868bdf9800fbc648f764ff6aabe878e837cf5e`  
		Last Modified: Tue, 28 Sep 2021 02:27:10 GMT  
		Size: 10.9 MB (10899138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb38129bed7931b18a48dcbaa75e8350149907c137d95496ab9e8fbb32aa6d6`  
		Last Modified: Tue, 28 Sep 2021 02:27:30 GMT  
		Size: 55.9 MB (55867003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:06b714e4afeeaf5a5ea67a0e493064f71329a8a8a9b01d40f8d5b0bc87b04e16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130478736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42882d2ad744ca8f780a934a350b370b9184646c9ba3a6fe87ec9da44ee3ae33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:17 GMT
ADD file:07dfd2960f3649fbe7a701ad0b551f48b4815ff5eabaefe7aaf62e770435e5f2 in / 
# Tue, 28 Sep 2021 01:42:18 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:17:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ed4b6e2f624e3ac187bdfdafce616f76387ede25afbec70c204c9d6300d2e0`  
		Last Modified: Tue, 28 Sep 2021 01:52:05 GMT  
		Size: 56.7 MB (56733325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a4c8e238708f81b44eb4ba40b5c8f710f262c0c1745ffcdb299c8387dc061`  
		Last Modified: Tue, 28 Sep 2021 02:27:58 GMT  
		Size: 5.3 MB (5312381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e976216252ce09cde1548cf4c9a4e367e1cc4c4fee46d9a25408720edd938df`  
		Last Modified: Tue, 28 Sep 2021 02:27:59 GMT  
		Size: 11.3 MB (11282013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6ebec24d20e38092d845932f91387b27fb11b3740ba554966788b972768db`  
		Last Modified: Tue, 28 Sep 2021 02:28:26 GMT  
		Size: 57.2 MB (57151017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e7bbed7ac5659c6cd1aececdfaa4dc4744c5e258ee5c650a8ec37b539fda309b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124674074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f801a22581fced8c27b30a1378a19368e58a491bf7f4c84d59eb7a011e8343`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a709b007930a1acd8d8ea50132cb0b6a34e4f6f470c1b917f467d1263256229`  
		Last Modified: Fri, 03 Sep 2021 02:05:35 GMT  
		Size: 54.5 MB (54506202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a5c418dd1d0e473e559b3a703a9e40757ead45790002b65bfc2bb736e31a077f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136722538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf7cb6d58a64ecbd4e666e5dc9905f0bb6786a021d2c2d955cf233ab37f7ef`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a95302a54a7fa51cdd0cd0117968b05d9f71d3c40eafe66873816a3b43ba14`  
		Last Modified: Fri, 03 Sep 2021 07:14:06 GMT  
		Size: 5.4 MB (5422617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da11fea16e40da1a9b66dee60a49dee27fffb468c778b12670ed59f3cd11837`  
		Last Modified: Fri, 03 Sep 2021 07:14:07 GMT  
		Size: 11.7 MB (11650959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd39c289a3baa1fff8358db49e63fac02746752ceae177b4b7a19642ba640995`  
		Last Modified: Fri, 03 Sep 2021 07:14:30 GMT  
		Size: 60.1 MB (60114890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:f39ef8a4165175de61f83dc3174aa76194916a15f5137f0e1bf51f5b86cc7ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118627696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1485f61f1c24b7322dfb4b732919e5862c78ff48a917cb91cdae8e09b3e50e75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:14:19 GMT
ADD file:c8ff49735749af794fa2a6ca03eb4ac0fb66dffd4ead8d9902ee04483db97aff in / 
# Tue, 28 Sep 2021 02:14:22 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:56:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:58:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f903d1b59452679ad13935f22aa7eb73ffa71398303161a843221e41855e5bce`  
		Last Modified: Tue, 28 Sep 2021 02:30:17 GMT  
		Size: 51.5 MB (51531137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec6ba981ab80c88267fed9b741a2a2ace934d0bb03930338f0126518120a416`  
		Last Modified: Tue, 28 Sep 2021 03:35:59 GMT  
		Size: 5.0 MB (4997888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736a4b194f9d38dde15b4c734cd79228a198fb0314eed4526e0135d4254874b4`  
		Last Modified: Tue, 28 Sep 2021 03:36:02 GMT  
		Size: 10.3 MB (10314682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36c310fdfaed216b6a43fd07fe77c729b8d8abfb8772e830cda42b0cca7024f`  
		Last Modified: Tue, 28 Sep 2021 03:38:07 GMT  
		Size: 51.8 MB (51783989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:32b95e6cbcac8947758c681cc7c6e8995abc6b755ad8853070676f621ccf168b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125072581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d879c30c528729314fbb2e692c8bfb507fd458de13198f1af75a320ad2fd8d7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32362b87984c1bba14b0f80546944827886c7cc7accd0865b4ccc7f34a9f3b8a`  
		Last Modified: Tue, 28 Sep 2021 02:17:31 GMT  
		Size: 5.2 MB (5165065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aadefacf33492b3a74622a982ea04f1605a554feeaa2ef0abdd214a94280744`  
		Last Modified: Tue, 28 Sep 2021 02:17:32 GMT  
		Size: 10.8 MB (10793806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217921cacc4173d4ddbf287e61dbfb88ee91ded7acf28b93d6b7db50ca7ca75`  
		Last Modified: Tue, 28 Sep 2021 02:17:48 GMT  
		Size: 55.2 MB (55159873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
