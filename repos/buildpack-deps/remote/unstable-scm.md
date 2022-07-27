## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:e970d25963ae327858af5cb56c074aacc4570ef08f8ac123a1fbe6191be4af4d
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
$ docker pull buildpack-deps@sha256:42bdfcb48e4acfafbcd7969840b3931935dfc049ad6a11875f7db06126ee39b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131791649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d276c6c0a435226741bc7e8ee231e2339867418a4c397cfce7a622eaf42c830b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:07 GMT
ADD file:0aaeb8a0c7fde9f030dc2ab67a03f21f44e9eecad9e4cf1f360dc5f768292460 in / 
# Tue, 12 Jul 2022 01:21:07 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:51:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:51:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4a81bc091a3ce5ccc3c89ef56e710ee1854c5ff9fd3d7f148e87cb956b5b78c7`  
		Last Modified: Tue, 12 Jul 2022 01:26:19 GMT  
		Size: 53.2 MB (53226349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b567a2d645b715cf7eced5f75816db7c980c3416be39e599e6e4b0bbc82f9eb8`  
		Last Modified: Tue, 12 Jul 2022 02:57:17 GMT  
		Size: 9.3 MB (9295637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303c4db152401668239f15446f8107b320fcfdc241030fd93f94783340b469ca`  
		Last Modified: Tue, 12 Jul 2022 02:57:17 GMT  
		Size: 11.3 MB (11271765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cf65a8772cd0616a80dfa0049c8ec6ea822121ccf534abed287a6206d6e1ca`  
		Last Modified: Tue, 12 Jul 2022 02:57:36 GMT  
		Size: 58.0 MB (57997898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7714d745bbfd1bee0a659a5662658c4b97f0d4837ded37aed06c03ec7b64ff3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126405974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3011c8b5fd2e2a5933c1801d482c79b1cc2c68e44efbc78e6ae92e90714364bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:53:06 GMT
ADD file:d09e1e4b772f7be41e6f5adcb5a71d86548e6099876e8d5d1bf8eb816a2d8cf9 in / 
# Tue, 12 Jul 2022 00:53:07 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:47:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:47:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 01:48:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8fedff5488db39c94b1a6e628f1dd8a8718a76f0b9f0a65f57e06652448e9f4`  
		Last Modified: Tue, 12 Jul 2022 01:06:36 GMT  
		Size: 51.0 MB (51027952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdb9c4c566afe6ee79f348756dbd9b7b7752109285ecc12936279d515cc71f`  
		Last Modified: Tue, 12 Jul 2022 02:03:57 GMT  
		Size: 8.7 MB (8725449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece2169f6168d0cd57063262293e9a5e841d140a27a657883596ac7fb3cafeaf`  
		Last Modified: Tue, 12 Jul 2022 02:03:58 GMT  
		Size: 10.9 MB (10940756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50438d01e861fe384e7553119984ecff7f7b3803745a0459dac979d7b2f1825`  
		Last Modified: Tue, 12 Jul 2022 02:04:49 GMT  
		Size: 55.7 MB (55711817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cc3a1ab7cf0ee2b79f4a4f7ab163c70026b4319269f2b1e71d0727442f17a6d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121426826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ff4ffe8010f84d7d60cf12590f2f02c41d999e3755608cf00263244cbdba20`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:02:35 GMT
ADD file:d11763b9aa59da9e9615c9a7df09de9c36f21a814e568fc0e11405310a9a2562 in / 
# Tue, 12 Jul 2022 01:02:36 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:36:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 03:37:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8fe2658d6ff3dea5d2d17cac5d8ea95c2ad6ebd5891a981d88d937403638c1`  
		Last Modified: Tue, 12 Jul 2022 01:15:55 GMT  
		Size: 48.8 MB (48767592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073b6262dbfc4ae07e4b7e3e4239774c53b157a42dbd8ffcb7c6e9e122036e7d`  
		Last Modified: Tue, 12 Jul 2022 03:56:08 GMT  
		Size: 8.4 MB (8405583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a757a2ad0986080b4acea992995782caa9151b4dcfd8acecc382d0bf2ae7e33a`  
		Last Modified: Tue, 12 Jul 2022 03:56:09 GMT  
		Size: 10.6 MB (10585915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1b020f7ad450960e08c7cc53eef736f876605f45ebc85e1493194e9dc7b776`  
		Last Modified: Tue, 12 Jul 2022 03:56:57 GMT  
		Size: 53.7 MB (53667736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b6f942361c32ac509c6072cd18dd9e331b90968745942d3fa5cc3d6c6f940487
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130615124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53e9871c0346e9651e8f217b106fa21e1407e8c0be5e30a163241800ef3f9686`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:40 GMT
ADD file:0f18dcfe7e502abae9dd7f72911dda640e4675306760d63f467092f962228ad1 in / 
# Tue, 12 Jul 2022 00:41:41 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:36:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:36:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:36:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3ef27d3c918a6321957a64c33268d09a01ec18590cce79a144625d9c0c8599a`  
		Last Modified: Tue, 12 Jul 2022 00:48:17 GMT  
		Size: 52.3 MB (52331756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f3b169736466d16aa015562be48cd38804707291d997ad0a77f69293eb28a6`  
		Last Modified: Tue, 12 Jul 2022 02:44:53 GMT  
		Size: 9.1 MB (9139825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fef5554fb71c819accf1cb6b60a439cb9c6a8da7ad329ecdfa59582ef1f116b`  
		Last Modified: Tue, 12 Jul 2022 02:44:53 GMT  
		Size: 11.1 MB (11056631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0f540b5927de78a3401234b3c45e6a2af90069da738315da30619808488023`  
		Last Modified: Tue, 12 Jul 2022 02:45:13 GMT  
		Size: 58.1 MB (58086912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:230b915a004079597cbd6346852581c73f3f8f971e1f48b71966e0baca47b7a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134611164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbc6a142e28bc4a973e93eb9d1e924ca982998548c266514f5a15db0b1d0d72a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:33 GMT
ADD file:f76df7d0d2c0977290a0183cbc4f62656ab20d04eb0cae4d075fd31ddf9df8b4 in / 
# Tue, 12 Jul 2022 00:40:34 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:30:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:31:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 04:31:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7f5437d02adf5c6ebc8b31ebf7b4950c58003a838e1f6591ce754472a3bae43`  
		Last Modified: Tue, 12 Jul 2022 00:47:20 GMT  
		Size: 54.2 MB (54207595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd45fde68a9a7357df097d16053cd6c09bd1e8e11d9a007f639e8450c6debc88`  
		Last Modified: Tue, 12 Jul 2022 04:38:27 GMT  
		Size: 9.5 MB (9466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb688f237713e90f9618c949c97ebc2f9695bef669becebbfac33581372c6f5e`  
		Last Modified: Tue, 12 Jul 2022 04:38:27 GMT  
		Size: 11.5 MB (11469728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a41906da5caa475cd2fe52b2ecdb650a99dcb1b6fbec92456a583ecdd381e`  
		Last Modified: Tue, 12 Jul 2022 04:38:47 GMT  
		Size: 59.5 MB (59467468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:295a42175f906cf0f90d3e25ce3d6a2662fe61c561fa191cfc8f3e331c1adf39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128739233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b447b3e0d694f6c4a2c9ab778df025396639718cc8ecddafaf323c6a337d1c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:44:00 GMT
ADD file:f6825f1dd59126d26ef0dba330a1d0eff37f6b9d56fe4a1bf2669774a6a7c74b in / 
# Tue, 12 Jul 2022 04:44:06 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 06:27:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:28:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 06:30:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:043042ab5eb51d2e5fe9f7bf85b86a91823ebf404e02b09bd9d96e29066acc7b`  
		Last Modified: Tue, 12 Jul 2022 04:54:59 GMT  
		Size: 52.3 MB (52346196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78102f519b643046757a9cd4f6d008518ddaf7e24f82322dba5336a7bff1dd7a`  
		Last Modified: Tue, 12 Jul 2022 06:46:55 GMT  
		Size: 8.7 MB (8664834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf3efe7ae97a67b5d9d9a2fd74d9d6407dc893ffcf6df03128e98d57bb34138`  
		Last Modified: Tue, 12 Jul 2022 06:46:55 GMT  
		Size: 11.0 MB (11033383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347923227ed46aa579c468e307ffc94f47c04832fca5d90d1787e75a20df5a5f`  
		Last Modified: Tue, 12 Jul 2022 06:47:47 GMT  
		Size: 56.7 MB (56694820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6123c5ad7fa3716831ca5a739061ba89d728ec9f55210bf5e5423b131e251274
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141679433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f202865500436ef2096d89c6ec75ca84e8126a7b08c32a799b55e8b78531a958`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:27:28 GMT
ADD file:8039654bddce2cd83d9433d1df0a53c329e7877cc8210593bcde23de63e2f1fd in / 
# Tue, 12 Jul 2022 01:27:36 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:49:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:49:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 22:50:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0d4394941206b4f218ffa2a2b794698da5149ab7a22b52f71390aec65a7add3e`  
		Last Modified: Tue, 12 Jul 2022 01:40:47 GMT  
		Size: 57.4 MB (57441462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e13dc094f3be3cdae228630277f198c2aee4ccf4989e03df692829782575ad`  
		Last Modified: Tue, 26 Jul 2022 23:51:25 GMT  
		Size: 9.9 MB (9889588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9148c549699d52333ba063274d8397af520c8317b8d893c23ba0800047eb2b45`  
		Last Modified: Tue, 26 Jul 2022 23:51:25 GMT  
		Size: 12.1 MB (12082932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c97a942b806632ce20c77655f33f494e860c5c99b3cbbe88c8a6d4a5eda5577`  
		Last Modified: Tue, 26 Jul 2022 23:51:54 GMT  
		Size: 62.3 MB (62265451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a554d40bdf614dfd9e405a249dbfe2bff02cb93429ca042ff9db3c8e0b1c3124
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122419082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eef1028664b4597959820e5ea3724c58b7a5eff1763e4f7d9729c7729d13014`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:11:50 GMT
ADD file:e156d172727c94dd7b17970577469d9b556db67960762f454d5b90dad3f746bb in / 
# Thu, 23 Jun 2022 01:11:53 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:58:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:59:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 02:04:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70334332338a08f7ae515b43812936d5898e62e8ffd5fd38ba59761c5ed137d9`  
		Last Modified: Thu, 23 Jun 2022 01:30:12 GMT  
		Size: 49.4 MB (49429796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5fc26886e551b626bc82f99096f4659ee9ee5af689dad0d03fc75d88c37d88`  
		Last Modified: Thu, 23 Jun 2022 02:51:42 GMT  
		Size: 8.4 MB (8394795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6176147b43ca0f721514815cbe526cd0e19723ed30c23a9a3534a95d32d19cb`  
		Last Modified: Thu, 23 Jun 2022 02:51:43 GMT  
		Size: 10.7 MB (10650389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebc8d66990654882c5fa423a1a4c713b77656fe3fb7540e4e51bbfcd8395d3`  
		Last Modified: Thu, 23 Jun 2022 02:54:14 GMT  
		Size: 53.9 MB (53944102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2b47118b90a37280981e27753473870698226c8236b58191eb832721da3affeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129131202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:453ace87d9c651cbfa6003070ecfc31e9bc0a4bb51c4a00bf9ff8d14a0250556`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:46:07 GMT
ADD file:160fd6ac1dd96abed2e1719ac95e75e8a8eeaeef9e04a353e0ba4a23cbd1c1e4 in / 
# Tue, 12 Jul 2022 00:46:14 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:45:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:46:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4ac3f896d9c36c21fdbee9a7ab2637136d4d09ef6db30c3b2b4ab10c48abbe7`  
		Last Modified: Tue, 12 Jul 2022 00:55:11 GMT  
		Size: 51.8 MB (51757401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7d0c4835633a8b04da06d28abb8af4b5557ef25b136337b6872fd92b710b70`  
		Last Modified: Tue, 12 Jul 2022 02:55:25 GMT  
		Size: 8.9 MB (8939218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabdcf7f5d4d109945eb55d7a1fda36ddcf55c65eaff794d0456ee0e0e2e30f`  
		Last Modified: Tue, 12 Jul 2022 02:55:25 GMT  
		Size: 11.2 MB (11162924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bdd31018381fccdd1cda9c7f537afeb37f464aeb418cc92baa60a4b3a165ab`  
		Last Modified: Tue, 12 Jul 2022 02:55:41 GMT  
		Size: 57.3 MB (57271659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
