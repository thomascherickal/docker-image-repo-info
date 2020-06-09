## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:d6e3ebd8489360b4a594089ff9b73c17fb6b512673ab3273a17803ff477774eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1b89cb27acb4aed5fffeb484b3e1d8f127f847f803cbfec7328252d9c1f62834
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69822078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6a2bd2a17080d7fb6a5607ad88d2bf40b878486867545c7d6fadef8c15c2c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:10 GMT
ADD file:5c0c0fbac6fe503c1d3e894e0b3b1081172862074ceed378a7e4b82810536415 in / 
# Tue, 09 Jun 2020 01:20:10 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:44:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:44:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:07f1101e3e85b531862163b4177bce7f401eac107a6537ab74195b395aab30b7`  
		Last Modified: Tue, 09 Jun 2020 01:25:12 GMT  
		Size: 51.4 MB (51413507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3778b8917e949d9f5a076dfa475de8efd560f3537663e53ea97e720164dd04a8`  
		Last Modified: Tue, 09 Jun 2020 01:58:55 GMT  
		Size: 7.9 MB (7920377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4483e6954e0bd5f111c062eb05965cd7e6719912e726370891437022744c5b6`  
		Last Modified: Tue, 09 Jun 2020 01:58:55 GMT  
		Size: 10.5 MB (10488194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:83a0de29e0bfcf59052c7040734e759700787343f82ad8b070a27579f8606d23
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67062742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f50165b074c55d93d6872a047076912372d234aafd6ea6aba8eb8fec1fa21a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:50:42 GMT
ADD file:ce6e6e497a66e2260260f97fe2b75c1b96d64554c5be6b85940fc97e2668da58 in / 
# Tue, 09 Jun 2020 00:50:47 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:23:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:23:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0cdc268ccc707144d53d65848999b81d39614c650312788e7e7f99c56bad6d97`  
		Last Modified: Tue, 09 Jun 2020 00:58:27 GMT  
		Size: 49.4 MB (49386621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86dad966a8a2c2ed7fa83ce42c1fab459f250a20c801eeaf7703e5022cf7bfe`  
		Last Modified: Tue, 09 Jun 2020 01:56:29 GMT  
		Size: 7.5 MB (7500258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5380110dfa23bbdc9c556dbde735e0c5c0b768f93dfc86e54d0c9e2adb417562`  
		Last Modified: Tue, 09 Jun 2020 01:56:30 GMT  
		Size: 10.2 MB (10175863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:84983f7c7e4ec1162e1ad7c65bb617f9ee37f9eb47f88c059bbd6f09ac864213
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64264342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9cf75dc7ed007a9b9a9e3c6ecd46e28009e4533d8965f519b9370f132c96eff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:59:35 GMT
ADD file:2ade41d5fab2319a3cbf973cc24aec4f6b9e2b14fa04578886fa1cbe30e511ef in / 
# Tue, 09 Jun 2020 00:59:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:37:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:38:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1c27049a799a3404864ae1732d5aeaafaef7ce0fbbde552819e2c88bf38ae9da`  
		Last Modified: Tue, 09 Jun 2020 01:09:22 GMT  
		Size: 47.2 MB (47197823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b26b1bf1a6c82f64fb3246383f0e2081a0624861a1d56ae6b025e7406652be`  
		Last Modified: Tue, 09 Jun 2020 02:09:55 GMT  
		Size: 7.2 MB (7243223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ad054395bdad7163609959df4dbaf402b1787fb76da08b5c5f89358ac9f2e1`  
		Last Modified: Tue, 09 Jun 2020 02:09:55 GMT  
		Size: 9.8 MB (9823296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d22c21bafbbd1ea61cacbd5feed91da07b7b75455afb7393a3ea90261903d7e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68644493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04707f97d47f3eb96b6295744a7c3cdfc437c1c1dd6f4052719c6be43d35bb58`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:50:43 GMT
ADD file:190cf77e9edc842728fc8939ff800920791bbfcac6cd73f98256162a878bd0ec in / 
# Tue, 09 Jun 2020 01:50:48 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:27:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:27:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:236f522da1693cf3f52676f554eb9aceb6eef7f041f0bf25655f0a27a10b2f41`  
		Last Modified: Tue, 09 Jun 2020 01:57:18 GMT  
		Size: 50.4 MB (50353814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404621f04a08a178357183de34af7ad63ce5ff53134378a1a1a442b05b443b74`  
		Last Modified: Tue, 09 Jun 2020 02:45:45 GMT  
		Size: 7.8 MB (7794925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61152c256fb5df63e0988148af095da2ef748b80883c73baaae8c4b7456a9132`  
		Last Modified: Tue, 09 Jun 2020 02:45:44 GMT  
		Size: 10.5 MB (10495754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a3dd76124da59ffd6f07fcb63ce24361a044dc458090d8597be1ec54dcb5839e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71491346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dacd4fa961e0f16c25c10005b021fd6b8187cd2f0b4c39391c467a33760f002b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:02 GMT
ADD file:8b8ef4a5f8149eba4e2e5c50f0e95fcf5b9e729c8fdf74e04ac12871a5e80281 in / 
# Tue, 09 Jun 2020 01:39:02 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:09:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:09:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e2c89c7c8738f073b61540c4d15c26608d6fa4a9756e727acf258769f4f15726`  
		Last Modified: Tue, 09 Jun 2020 01:44:12 GMT  
		Size: 52.5 MB (52522870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68ddf662651a633a2f0e4f65ad7228c24d57d8b14286a1b62fac342f6375f75`  
		Last Modified: Tue, 09 Jun 2020 02:30:14 GMT  
		Size: 8.1 MB (8099334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efad6eefe2105d3cfe168434dd0f3ae253e5013636bf2e2cce89b8545995ea84`  
		Last Modified: Tue, 09 Jun 2020 02:30:14 GMT  
		Size: 10.9 MB (10869142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6168b7c1602a61c3ee33297a956b8cb7ed179af43412c99bcb982951728a8c46
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68114967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5979abf488ef443bcfb20d48981fde2897a26df2a7930fb8c2412e57a3231916`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:08:53 GMT
ADD file:080fe104a5c84718f0c41015a3a4bf48ef0d94088beb50e3b0346ea572302008 in / 
# Tue, 09 Jun 2020 01:08:54 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:46:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:46:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4295b4a99b75e24118d0a604e63b142af1639be17451d6724215fd11e6fdd041`  
		Last Modified: Tue, 09 Jun 2020 01:16:09 GMT  
		Size: 50.2 MB (50162108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6b19c74224bd3e9030de803cd7b2cf6f938ee3548998819522a786837b1caf`  
		Last Modified: Tue, 09 Jun 2020 02:06:44 GMT  
		Size: 7.4 MB (7447679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e65e61fe718bcf10bce9dbbedd4844ba55e178913be199a5e4cd26a5ca17f1`  
		Last Modified: Tue, 09 Jun 2020 02:06:44 GMT  
		Size: 10.5 MB (10505180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ff96ccb1581f10a5e5b2c8aac3e45cddd4e477165af7a593e003ef4f70e5ee1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74643973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed75f631222c95416bf21fac81e046bcf15366c944806a08b7a22de54ddfa6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:16:05 GMT
ADD file:890f814706ea242af3d8f4b729aed7d590611deabe25d4adae7468f0058d7a4c in / 
# Wed, 13 May 2020 22:16:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:29:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:30:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f2f9956082054d1fabd5ea1a9e08b145fa7f68b93b5601b36e05386466487664`  
		Last Modified: Wed, 13 May 2020 22:56:07 GMT  
		Size: 55.1 MB (55110307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9e43969f6c0ff55aa4240214980deed196b68292106e0144d8d1290495d9b7`  
		Last Modified: Thu, 14 May 2020 00:25:02 GMT  
		Size: 8.4 MB (8356860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eacce9e1d274d8f139e9d384ceb5e66a86ca1857d025523765b1b099330719b`  
		Last Modified: Thu, 14 May 2020 00:24:57 GMT  
		Size: 11.2 MB (11176806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e550f5afbfdc1ef0e1ae45ba5d46a3efb8f2074e47b99bddd9d2433d3cf8d653
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67973510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9980047f717a591b8ea934bd70ad19c7e12b4b32941d097817e2bb3ff3c3071c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:41:54 GMT
ADD file:336fb2c808ef96709e7e692ea601159ca29f93c7988099e297914a1da2171aed in / 
# Tue, 09 Jun 2020 01:41:57 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:06:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ce762a1b284e798ef27a5aff0cba859d84a0fba00f59301a1163551445244322`  
		Last Modified: Tue, 09 Jun 2020 01:45:51 GMT  
		Size: 50.0 MB (50017615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50ae223e3890552865d89503593412dff73329ac57a5e1550cefeaed9e23915`  
		Last Modified: Tue, 09 Jun 2020 02:17:11 GMT  
		Size: 7.6 MB (7589158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63065300ca352f26ee91c5fb6965d3499bb2bc95f1f600246e2c04629eae948b`  
		Last Modified: Tue, 09 Jun 2020 02:17:11 GMT  
		Size: 10.4 MB (10366737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
