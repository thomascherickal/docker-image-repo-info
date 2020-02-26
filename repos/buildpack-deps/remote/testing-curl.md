## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:86a3b723e4bd7f2f1059ddf36e18f0dcf9856ff366c3bd017382a602e4798185
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7543fd116b1e842b1385c55b49a5b46db75fcf71901d0c85381d6d0897d7425d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70032674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b1a6ddba16e1853e1bb2855a82b3232567dc60d5122a699010bcfa9421e4b2b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:36:28 GMT
ADD file:7d01effeba890adb1756ba0a76c42c1dde5a189003943fbf4cb9fae0c0e1a046 in / 
# Wed, 26 Feb 2020 00:36:28 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:04:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:04:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a4501da464e996edc2ef85325afe9881a58061a9a35b142ca7f0ba598553e49`  
		Last Modified: Wed, 26 Feb 2020 00:43:35 GMT  
		Size: 51.9 MB (51852739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00055416d483b70a8fceb7d6e7685e08d5c76fd449df312352288b650f0a5f83`  
		Last Modified: Wed, 26 Feb 2020 01:19:20 GMT  
		Size: 7.9 MB (7921881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eab3db52671a6130df45784942f13ea891360cc3cd5d39ad4208321078246c`  
		Last Modified: Wed, 26 Feb 2020 01:19:21 GMT  
		Size: 10.3 MB (10258054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d4b17f48c0c86359bc0e5b633ba19d6d4a3d2a35d68914a0158a8ec42e23112d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67331773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b631d46ff159e165daa0b3d743276c9e329adddfb8dac73716f01767e718adb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:25 GMT
ADD file:cd3f4cae9b31b83faef159941db546ad620281a9de9ad8b4c2e2230e329f629c in / 
# Wed, 26 Feb 2020 00:46:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b5f1b944f6f81b9832613484a0ab69b94fc4d7e69cec7cf9246276a84f198955`  
		Last Modified: Wed, 26 Feb 2020 00:58:09 GMT  
		Size: 49.9 MB (49859431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2309dee70eab6e2c15144731cd3a34dc25e8045f43ccebd56bca46a938673eb9`  
		Last Modified: Wed, 26 Feb 2020 03:59:01 GMT  
		Size: 7.5 MB (7497952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ebfbc2424c96e6f6b0bd4ccb126243789b984e1df82dfcc07372cbdd3c2ec46`  
		Last Modified: Wed, 26 Feb 2020 03:59:03 GMT  
		Size: 10.0 MB (9974390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:93c2925c6cb8f7c58c2447f4684704fe094d27549ea7d975e0e1c425abcbc71e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64457440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d7acc7a1ac76cda28e524da9f79d3997a211f2a4e2811a15c44e5399766435`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:49:40 GMT
ADD file:516c2d0189c8132f97d954209787ec2c833e16a9d8a4056cc9ed22510c721b48 in / 
# Wed, 26 Feb 2020 00:49:43 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:07:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:07:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d46b4a12bd08cdd498cc190f7d350b7bfa151e105942f36a185990c238f53695`  
		Last Modified: Wed, 26 Feb 2020 01:06:24 GMT  
		Size: 47.6 MB (47581289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab620fe7c5ae5218251dd6127456072d85bebc5b47b3359937f36ce071d355df`  
		Last Modified: Wed, 26 Feb 2020 02:32:01 GMT  
		Size: 7.2 MB (7237740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba007f6e72abf7b8df1b3d1009db9b497e33953f02bd91c28566d6700b3e462`  
		Last Modified: Wed, 26 Feb 2020 02:32:01 GMT  
		Size: 9.6 MB (9638411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fe352cabca4e55106c8d709e1c51dd2d81c826d00ab4ce1d36e8e311431668e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68858556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5744862282ca211f3e8d579b1e179b9eaeca0f103f3d93d752f7d763b7858711`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:45:20 GMT
ADD file:6771f02669c2a4d080cd86fa10f39851d26351e4a29f9ff3d63a76e1865f96ad in / 
# Wed, 26 Feb 2020 00:45:22 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:45:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:45:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f822750796cfd016baf6c8125f67a171683174c26da351c46b78a6cc9d234372`  
		Last Modified: Wed, 26 Feb 2020 00:55:10 GMT  
		Size: 50.8 MB (50808549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f2d34813aa8b1aea79c2e14a664c47e0950cb8413f1af463215020fbe6ad26`  
		Last Modified: Wed, 26 Feb 2020 04:03:59 GMT  
		Size: 7.8 MB (7797144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74820b1316f035b3f4e91222feb71d75980d5a8b243cd3ea1a4ef519acca4774`  
		Last Modified: Wed, 26 Feb 2020 04:04:00 GMT  
		Size: 10.3 MB (10252863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4814d4f122759c37bcab812776332cfc798f720d210ba53e8d9aab69f35138a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71724477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01727a22bff09e14c1ae3432ed0d4228cfc4050f6a8166b879e4d3993980caee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:31:20 GMT
ADD file:d6037ec8e49283f4a0fd36cfd0bc4723725164526c4c56459e4c9f3d73c61d06 in / 
# Wed, 26 Feb 2020 00:31:20 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:04:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:05:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1d581a0f5f74a9924d3ed374e49a0171892551a9eef1c8d7efea523bdb4334da`  
		Last Modified: Wed, 26 Feb 2020 00:37:37 GMT  
		Size: 53.0 MB (53002659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095cc9a34f8e935c2fbfb4ac9eb3644923f64856d1434b4ac0f9dd4e3db91c92`  
		Last Modified: Wed, 26 Feb 2020 01:25:50 GMT  
		Size: 8.1 MB (8098985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab82912141b87280af1133876199f3de73be0b8797e7c31724505f58ede4e01b`  
		Last Modified: Wed, 26 Feb 2020 01:25:51 GMT  
		Size: 10.6 MB (10622833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:de813c0d181da76cd3754f9db008cac716029be94b36afb0e512de8a2dc04621
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74602762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a6f4823ca45daa64dda89e8df04896fa10c4c066a40465c0eaf33a486940e9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:17:00 GMT
ADD file:1a064022bd5caf45345b7a91191b82f0d2bb576e88e99652a4c3d68c399b1578 in / 
# Sat, 01 Feb 2020 17:17:04 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:25:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:26:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c80e92e9d0447b759db73a162ee40f56912d3ae4c251aa735339219ad9bc7a68`  
		Last Modified: Sat, 01 Feb 2020 17:24:16 GMT  
		Size: 55.3 MB (55316324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0367678cef47c5fbcdebd74948fd485de617cb36ea2d6182b1dfd3d5b1429b7f`  
		Last Modified: Sat, 01 Feb 2020 19:14:34 GMT  
		Size: 8.4 MB (8352503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc091c35bf183343a79cfcaaa09372d04e69e60e2bf829bb74249782b5c28826`  
		Last Modified: Sat, 01 Feb 2020 19:14:34 GMT  
		Size: 10.9 MB (10933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a002226111ff748fe440f194b839c58be9ebc8f8e28cd4c075646c7334200cdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67867003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d4689befce7bee2f34ccd9e6418edf57fe1dc808f3128f62b467e560d39ca0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:48 GMT
ADD file:cce6a1a9e391072489b92618430aad507d896a0892b4ab746b46f65aeb50e142 in / 
# Sat, 01 Feb 2020 16:41:50 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:48:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:821c3e818de5d8d85868e03fa7647e09cacd5ec4fc251a32c8469652dc6a136f`  
		Last Modified: Sat, 01 Feb 2020 16:45:08 GMT  
		Size: 50.1 MB (50133126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95eab022dfcbfcacdc7e34c79e2393c47272871cba3199d2f185d32eed6346`  
		Last Modified: Sat, 01 Feb 2020 18:02:40 GMT  
		Size: 7.6 MB (7592340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fc4d83f881a25a8f4d4dbecfe9212342061b813cb745e8c7fffaa872c5ce04`  
		Last Modified: Sat, 01 Feb 2020 18:02:40 GMT  
		Size: 10.1 MB (10141537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
