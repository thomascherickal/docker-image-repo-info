## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:d5652e275cb56452fbc7d83a798042b5a2d476f56d9eb95e699af9f00bda6ed6
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b814c4b12f8ea97e366d0d414c4570a34027baa36a795c165feccea2cd466681
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69782300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbaef275c24d20628215db0bfb0687938f6c0d81ead0d92d316af1f8d6c4e181`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:45 GMT
ADD file:19778292422b784c4eb17d79e7632fc1e3619b6bbbcf16a37bb6179a5c725b1b in / 
# Wed, 13 May 2020 21:19:45 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:25:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:25:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5ce4ab219a2f8bc551eb2502df5b719a1d8a32c4bbb00b3629001ebb6c5e0b94`  
		Last Modified: Wed, 13 May 2020 21:25:41 GMT  
		Size: 51.4 MB (51384672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f458d7d6918561d3665fcf7c6a15ac5f015d15f94fe4c18152b31a6b390477d`  
		Last Modified: Wed, 13 May 2020 22:43:48 GMT  
		Size: 7.9 MB (7934430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a19396f1ca9e830aec22ccedc673036a5d9fa5707ad170217dadb18689b7f61`  
		Last Modified: Wed, 13 May 2020 22:43:48 GMT  
		Size: 10.5 MB (10463198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fe3d0c4c775b38db477323f0745b0d9a4c0afdbf53b4e80987fe365d81a73715
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67031360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c6ca734fab60ea981e67aa1392ee7da511f7e157d32db62c99929ceb9f7b64`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:36:28 GMT
ADD file:099743a0547d5c892b4a3daaa3fc0f05d8317cd4946a0e9508d130ee56db63bb in / 
# Thu, 14 May 2020 22:36:31 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:38:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:38:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0238daf30887e241cdd1334fa6bd5883d06738c7ff61cea1b32a3361de098564`  
		Last Modified: Thu, 14 May 2020 22:45:51 GMT  
		Size: 49.4 MB (49359451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f1dbc2de2b0cbdbc9ae5411e2efb20958587e0c8691a15a5755669fe35e467`  
		Last Modified: Fri, 15 May 2020 04:00:22 GMT  
		Size: 7.5 MB (7514224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4b62e0336252e727cea159b040a0ef9263bc7ec15d9411459056795050f87`  
		Last Modified: Fri, 15 May 2020 04:00:22 GMT  
		Size: 10.2 MB (10157685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d8606c820869373beedbf43fbbdcf277d5fb88957105f8d390cd950df4ef3a98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64223985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80bf8e51b8145a40887b71f97e09fe178fcd6dfa6fe670f0bd411dcb830078ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:12:36 GMT
ADD file:6043fa3a64fc1fc92478b236dc9d857c2a161dafe05b2c17c95d16215a7488fa in / 
# Wed, 13 May 2020 21:12:40 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:51:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e3d0ed714eb8acd6cc43ddf13830c6dbe31523db4962134b70f31da0774c2de6`  
		Last Modified: Wed, 13 May 2020 21:22:37 GMT  
		Size: 47.2 MB (47162349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9410321c9d6846391c2c00276788966a82b6c2f4e1cbd96f8417d39b2668cc8`  
		Last Modified: Thu, 14 May 2020 00:18:46 GMT  
		Size: 7.3 MB (7257008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c897e7828d6f38dbee8e4f232bdd8c3fa793f6b47f6f6c5475f1129bf3abdaa3`  
		Last Modified: Thu, 14 May 2020 00:18:46 GMT  
		Size: 9.8 MB (9804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:311fdb6981c18e410d1949ba445947b5248817bd039fe478433c50c2e35f4c09
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68597729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5ed064da5c58d7061a77c07247909806ab8778faf7d1f66a1e1d229cb5c91b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:52 GMT
ADD file:642f1f8b3928c38913b91b5770e5ef77e0467db31d0e7342848c66b97b0cefce in / 
# Wed, 13 May 2020 21:41:58 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:19:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:19:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:da14fdea4bf7eaa36b82ecde9ee461379c7eb32fac279c7d1bce1452edd5bf2f`  
		Last Modified: Wed, 13 May 2020 21:52:10 GMT  
		Size: 50.3 MB (50328349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d18f3d952fdbc982edca77fab71409bebc6a0b410a5f13ffe6fd2685b6020c`  
		Last Modified: Wed, 13 May 2020 22:38:11 GMT  
		Size: 7.8 MB (7809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382abc5b67b7c0e46916f728a90e7aa0866070c3a67e581de6b5904092e6ca45`  
		Last Modified: Wed, 13 May 2020 22:38:11 GMT  
		Size: 10.5 MB (10459917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1861e1408f83b83c01e5dc89e9370b84c90e7f09e8dfd228306bbaadcd4dd0fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71433678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4424f1f7b269f611056a3c4e9aa8708b820902e8e8b00f21926c03c82a811922`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:38:36 GMT
ADD file:ad345e25a8b64e5d96a8875a8c7eceb747745ed11d495c0de132b2a33e48e29d in / 
# Wed, 13 May 2020 21:38:36 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:39:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:39:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:424ac85ac099fddf73c8eff4a7e1e7a3ad318011cb2070285233ed10f3794d6f`  
		Last Modified: Wed, 13 May 2020 21:44:40 GMT  
		Size: 52.5 MB (52480291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cf73924a61888429404a98bf52d320053b3f0ae8798a7c67213f15e472cc5f`  
		Last Modified: Thu, 14 May 2020 00:00:27 GMT  
		Size: 8.1 MB (8112084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1954931eaa7cbd6f17b8d579de74c26f37b042c1f3ce12b5d23001279df88d72`  
		Last Modified: Thu, 14 May 2020 00:00:27 GMT  
		Size: 10.8 MB (10841303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:438cad60c0a524db221018fd50e2a3b3f0784b63acaeb96b9a2c8bfa8da3a0fa
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68076797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5802ddbb3e5652e764abb13b97d472c806d40c1c6035a9111dca647a6ad37725`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:47:32 GMT
ADD file:f2d8d152f2c12223430241ba470d074182fc4071fbe07696ef9a7ac73d7e31c8 in / 
# Wed, 13 May 2020 22:47:33 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:50:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:51:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e9fe8ffba560af94cfc9c2199a294b5143a198e0cbe44469cb586e1986f063ea`  
		Last Modified: Wed, 13 May 2020 22:55:41 GMT  
		Size: 50.1 MB (50131081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0640353f1b9db4814a57a569a8417ac7dca26baae0a3342a2575bad188f9e2d`  
		Last Modified: Thu, 14 May 2020 00:11:53 GMT  
		Size: 7.5 MB (7460937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce2184377077db50bd5cfbf56505a742cce1db802c2fa42946c103a34a61969`  
		Last Modified: Thu, 14 May 2020 00:11:53 GMT  
		Size: 10.5 MB (10484779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

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

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a45df0c708c032a0d468804feb0bc736655c9535d8c8caa52f5524cf7f30531d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67950987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79054d0eea77f9cb5c6984e0dec031e24d11e204cf3e30430879de98cd58e1ef`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:05:50 GMT
ADD file:56a2d8bf46ec4edd3d768966ad8e9b4c86561cbcd482ae49fc18cc34306d54fb in / 
# Thu, 14 May 2020 23:05:53 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:58:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:58:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f0cbd757e4d594cf3793c18e1f7d5d6f3fd983ea05bd2edeac4774c47e85b763`  
		Last Modified: Thu, 14 May 2020 23:10:41 GMT  
		Size: 50.0 MB (50002620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb69a5809930b7b8812ae832cb600c60afe5387c53903bf422ae0e80ff086583`  
		Last Modified: Fri, 15 May 2020 05:07:54 GMT  
		Size: 7.6 MB (7600625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd25c680ce576408f8c9a5e8891ea37ac21483e932a4bacc4b744cad80a975e`  
		Last Modified: Fri, 15 May 2020 05:07:54 GMT  
		Size: 10.3 MB (10347742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
