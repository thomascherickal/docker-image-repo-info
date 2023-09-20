## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:0eefd79c930f92310d661d456757d5164734e6c36f746ba85f96a538e84a19bd
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9a86b969123ed37981a0cd0a93181931761cec31968cf89f12213909c6a1773c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138510583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:213f7e04cd613d30b05f714ac08d1ed227b226295c28bd8b30ff047b4965aa42`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:17 GMT
ADD file:bc0b5b71ee53adf6297821668404ace4f79c4256461b99497849721dbd8e86ae in / 
# Wed, 20 Sep 2023 04:57:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:25:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d036181e87bed9eb2432498f0ccbf7baa06719a2d8360c3bc9c496bd9f853a7c`  
		Last Modified: Wed, 20 Sep 2023 05:03:10 GMT  
		Size: 49.5 MB (49482728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1e6c60efbe0c0012665a19f7b4b47dbdad105e96128f40794e9aa23e0da2c`  
		Last Modified: Wed, 20 Sep 2023 09:33:06 GMT  
		Size: 24.3 MB (24333156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28922a0c46a328800d30ba9ed43a2347d3d2859f84e5f14eb9a375ca7a20e3bb`  
		Last Modified: Wed, 20 Sep 2023 09:33:23 GMT  
		Size: 64.7 MB (64694699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f3be4b7c1e0a6b6e7992308a0c43a6a88a85bfcf90f5d81fa04d06f9ab6d5431
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132544805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01fb2ede4ba77358188778bd510bb85b1e8700bd418003550db50645f6ec0e43`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:51:01 GMT
ADD file:4c775ca1c9a8c87b9e1d380ae08f73f13d6c554601a5b87aef7f73b399316a50 in / 
# Wed, 20 Sep 2023 00:51:02 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:59:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:00:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af64b4d6568f99d4aba6c0cd1799711a18174e7c92ab564f1783b1b859742070`  
		Last Modified: Wed, 20 Sep 2023 00:56:46 GMT  
		Size: 47.2 MB (47165885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6ad399a5730010d73ad40e178b7766f2f23d621da8fcbfeaa0d9b45877a92`  
		Last Modified: Wed, 20 Sep 2023 10:07:36 GMT  
		Size: 23.0 MB (22966714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d774b6481cfa6a90dbdb4c1195266ca5258843ac16be4271bc6b26b545c6a023`  
		Last Modified: Wed, 20 Sep 2023 10:07:58 GMT  
		Size: 62.4 MB (62412206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d1c5159a907ce955d1a542f88b087778e8a946270e284c7e472c75d282c97fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127733940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb4dc11f8b6a8d147e6635cbb5e17f8ddd240f89b8903662255229d9de89c6f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:59:28 GMT
ADD file:48b9003b5f16cca577ade266eaa0f16a82c1470540f591ca5b3478846402f252 in / 
# Thu, 07 Sep 2023 00:59:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d85f55a7a6c774695f75c1a7ec0bc0caeb915349d9250d2f4e6737e12fcc92fc`  
		Last Modified: Thu, 07 Sep 2023 01:05:21 GMT  
		Size: 45.0 MB (44983245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b914bb1a1428c8af17f4b5fe2002cd56706f2764ffe325bc5a8693a2d5885cd`  
		Last Modified: Thu, 07 Sep 2023 01:48:19 GMT  
		Size: 22.9 MB (22863094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cce762d527587259cc24735a7095b0706f16c46d1015868fffe9995eb694b6`  
		Last Modified: Thu, 07 Sep 2023 01:48:38 GMT  
		Size: 59.9 MB (59887601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e9c3b2a5ae3f24276dbb485bfc8a1caf21b382087fe102cea9e455ba0492cccb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138168956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3e67ad7347a375afbb38549245b8fefa4de454065f16937a90613a1aa9d7a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:16 GMT
ADD file:3493f4ad2710629ee9ad4c981682b2afcc1d9964cb5034de77189556f0c0e810 in / 
# Wed, 20 Sep 2023 02:45:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:28:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d83e3b52cf7f7a250777a05d8d2d7960fd6dba8a6438beed3879ff3c389bb01b`  
		Last Modified: Wed, 20 Sep 2023 02:50:04 GMT  
		Size: 49.5 MB (49450488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3c1d25120e8f2e9e343e08182a50d4c8702fe0c41bd340742c6b29f86d2bd7`  
		Last Modified: Wed, 20 Sep 2023 09:34:51 GMT  
		Size: 23.9 MB (23885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9a4b96724b03d813d1d7221957e9975fae576e911ef75a702924957cd7ef59`  
		Last Modified: Wed, 20 Sep 2023 09:35:07 GMT  
		Size: 64.8 MB (64833249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:61f1734eb7cc2dffcc102632dc09a5bf8eac4d56b528e6fef08623fee11dada6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142841779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a0a20c531aafa83ea40d559fdcadaf5013136e02231a348bc42f44d62956c19`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:40 GMT
ADD file:ff611322e6674f9fde9d60d146cd9f1206176a7ad0bffa135200bb5ce18ef6fb in / 
# Thu, 07 Sep 2023 00:40:41 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:32:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:33:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e341a6bda5bb8b3c55cc00b75f2a70088193c4ac06611dc91b32f6ca7c58df58`  
		Last Modified: Thu, 07 Sep 2023 00:47:07 GMT  
		Size: 50.5 MB (50501474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199c1deb7fa20bc9fa5f1c71efb48e77dbb9169e65a80ee76e1af76eb11ef7bb`  
		Last Modified: Thu, 07 Sep 2023 05:41:15 GMT  
		Size: 25.9 MB (25854651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bdb07681e939562c846b9666284e56c74395ac42f0c90225a11e7174a6a41e`  
		Last Modified: Thu, 07 Sep 2023 05:41:38 GMT  
		Size: 66.5 MB (66485654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2ed02c5afc812e283e49488df73a5333dad23564f7d501700cd380babb708be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137511760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a286e41e2b73000aba3e8f5b518f8ee3ff06d41f06e562199fc9cc02a96565c2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:12:16 GMT
ADD file:a0f62fb4629026abfbc8955434580788fb6798315ec2cbb9fff3b490cae4ae5f in / 
# Thu, 07 Sep 2023 01:12:22 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:01:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:03:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbf3aa413814601f6b34fe509eeee19b8570d10547318d9e50b786a1305da8f5`  
		Last Modified: Thu, 07 Sep 2023 01:23:38 GMT  
		Size: 49.3 MB (49337937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57139e98311e15a5beb5188d286eb35893fd7b66379668ca38afc3c3926810`  
		Last Modified: Thu, 07 Sep 2023 04:26:24 GMT  
		Size: 24.6 MB (24560622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe5e62077ec632bacdfa13759bc11189801d913e3ad23d63f1a3c430854c2b`  
		Last Modified: Thu, 07 Sep 2023 04:27:16 GMT  
		Size: 63.6 MB (63613201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b17003439bafb15ce1952eb66376844a5b0faada93745abfbc232d5a2cd31792
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.7 MB (149685352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46c26819ac5b7a854adab36b150ac69ce02922bc41111eb02dac4d0cf380d5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 07:54:20 GMT
ADD file:cdb28efb46a4441fb0c394ab6cc1dc2932b94e5af87d436319c9c1f7be36c739 in / 
# Wed, 20 Sep 2023 07:54:23 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:00:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:01:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe32f2ba77f5d8b224f7db94357a292203e69ae2f9a815b5aecb41517006d3ab`  
		Last Modified: Wed, 20 Sep 2023 08:51:55 GMT  
		Size: 53.4 MB (53397269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371cfd6d9bde7f492d0557b8056722af99aeec7719a46f7523e196af4a49e416`  
		Last Modified: Wed, 20 Sep 2023 10:23:48 GMT  
		Size: 26.0 MB (25976696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d4b968457b19c383bfe9ecb0826c6b5224b515e8f8b8632474ee77c61b2454`  
		Last Modified: Wed, 20 Sep 2023 10:24:14 GMT  
		Size: 70.3 MB (70311387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:64e319eeda0d554ef44266fc87912340668bfd5ac9992f99539ec8b0c9d2e723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137893055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f00dd819a996fe5fc929dad0fdb9a654103cd5aae569b9b5468234731ab914c1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:55:43 GMT
ADD file:aeb19ed2c9b92cbe76bb1e733b04de5bcb32489c00c1c06504aef79cd36c3c3f in / 
# Wed, 20 Sep 2023 02:55:50 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:53:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b1b4950b21705690e4b15e5257a0efcf7d334776307aaa893216166a5c37f2c0`  
		Last Modified: Wed, 20 Sep 2023 03:01:02 GMT  
		Size: 48.9 MB (48852678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bea1485478ab1093cd60cf0d37627157771e79e9a675510ea1e4233d2499a85`  
		Last Modified: Wed, 20 Sep 2023 10:00:18 GMT  
		Size: 24.6 MB (24576163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248968c69731e8439bb01eea6789e1dd63c573a1c9e2be9c33d19b9a4411e465`  
		Last Modified: Wed, 20 Sep 2023 10:00:34 GMT  
		Size: 64.5 MB (64464214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
