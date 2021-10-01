## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:0ff93d51e83675d401c67c79e63e476d548b325b652aab348e14f616711390bf
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:876cfe58c039fd813ff318d4e53e2707c884cb7b8c7952464dcf2e27cca17b5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71783901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:506d6fd65061be41934c131b48e3c840c7e841b27244c6d3c657f0c4008db311`
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

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e87ec835044393c77ab96a3c4fbf5d4f999fe5c2aea983a35c8a24f333106911
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68903410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9a5d7085c78c1d80020d21fdc2bfcb29fe53b22a93b588e0d67af242ef17aa`
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

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ec123566e37f91cf7dc999a213d362dfbf1413d9ac4ad6232d3bee77c01ca4c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (66019179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f8848536df00d83694de40159ebe8595caf2bf001797c4d47dea972c82eb99`
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

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3cacb2497db42e4160cef77ad2ebed9249918ab55507fe1ca75a48a3b384ec58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70793889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e7747dd728e45e46bfbd2d710d52a2e130eae3b33fc78392bb548807e00939a`
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

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:138dafec4d1ffcacfb0d88e1ec201cefc8e953f8e5e2b566dc381409fe1df3ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73327719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0a6347fe9bfe440f7f7bee5c7628ea6b41d05955bcfc1e8025699c51acd5cc`
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

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0742b4ef0a1e6d36f6a1baf7431d7ce25444bf9575509f0ba031b8b243cf1251
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70167872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fac613c7b4b40ce813d10d55b6b0ad58587ca17e308844e5aa980796ab1392f`
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

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f686e9380a7ddf6bd2900de9f550ad307efaec5625ed23c223f0bc49e5b4eb11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76607648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:458f349d2522ffbef1b1dc6a5f6f49b9c4cec344f768cabcf7a36baec2536acd`
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

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0a6ecb3329f5b8d000b8e6e5e10ff4a66e34755b3f2f51f80bd52ee98f763704
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66843707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ea89476054b4f64f3f7013eaa3d25bfdb786c2b2a83de0b362dee8da2c37c0`
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

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b734c11fedc4319a44595c49e3541d7a69e4c3bde2e5b12f1082ed915b59a556
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69912708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f80b8e561ff61c6a6d9bd4db8e89f29950f901bce96b85d1b662f440d23f5c4`
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
