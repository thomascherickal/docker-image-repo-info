## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:a9f4d8c3b7b3a2dc0df98087234e6f2eaeb071875b284db6edede368c7beeb25
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

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9fe01d3c96732b7a430aff1337ff4a0bcae707d7b5656798e296706bacc200ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.9 MB (124948292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13f8b600931556bb7c0104446dea63955c6d29c11404531711c47d98c9e3263`
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
# Wed, 26 Feb 2020 01:04:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:74a471741589e2b8271d8be85e5a2d0ba4eb2667b7207711b99787dc20fa3eb6`  
		Last Modified: Wed, 26 Feb 2020 01:19:37 GMT  
		Size: 54.9 MB (54915618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f29e79c81253858970fbda7a0e9add80034c6cfd062c9bf81d48fb2e16b0ac40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119929632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0831f7f405f6df21d084531edf4ca391b13b0c907715fb18cf6259ae83ee242d`
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
# Wed, 26 Feb 2020 03:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:aba36494b890743c5415594ee83949a59b8e97262545880ca23c5428e07c583d`  
		Last Modified: Wed, 26 Feb 2020 03:59:28 GMT  
		Size: 52.6 MB (52597859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:90b6c33f5b3737f79f36d227073b2a78f7fdd49e947845bd3f6b4ba7c04601c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114789632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04cca46f3ba333c128d86d9afde8ce628cae2e4cc0e011a9e135fc382c86a36c`
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
# Wed, 26 Feb 2020 02:08:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:2db97fc91eb5d6d855e20ee37328160b266216205b0e2f0b9dbcefbb09c48b38`  
		Last Modified: Wed, 26 Feb 2020 02:32:24 GMT  
		Size: 50.3 MB (50332192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:24983c0a5ebb8379372492474099903eb62fba3a173fc6448daa38600366dcb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123983454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba51b4b050059cc797014e2c136735bc5c32be10ef7a2eb2e8b7b49a8967c4b1`
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
# Wed, 26 Feb 2020 03:46:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a934273fe78141239ebcd7f15bd23d865d400ab5e8f9a91732fa22672bd4308d`  
		Last Modified: Wed, 26 Feb 2020 04:04:23 GMT  
		Size: 55.1 MB (55124898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d5587600919ae9c3a81e4e8c551ffa41afaf6d1f8ea6b6f67c50f8615b67f2a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128482005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d54438f7b5ff6c2990430ad1bc4f6cb36b2769db08de534a7b8e0b1764e222`
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
# Wed, 26 Feb 2020 01:05:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:010e0c448a96676d2209e4a820484ca9c98f8a0cc07d29c7c7cf70b27ca66976`  
		Last Modified: Wed, 26 Feb 2020 01:26:14 GMT  
		Size: 56.8 MB (56757528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0d518e5bb7ed38649d15d72e06a735f17b496f740d9a002846bb923aee90eabc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134403777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76ac93e765cb2e39346dcc078b306359a1c2fe1c59ee971ab9be660b39ee118`
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
# Sat, 01 Feb 2020 18:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:30e665ecd4edbee998fa55d04d8629974e0da14b478ba821db4e2a9cda1bcf25`  
		Last Modified: Sat, 01 Feb 2020 19:15:22 GMT  
		Size: 59.8 MB (59801015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9404c912825554eee11294b1c46e95687a4ebec17ccc064af7391e81a9affe64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121671307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b415ba1d501a3a7ede49869fa5e87f920c34e36a378375d42358f3dec82dbe`
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
# Sat, 01 Feb 2020 17:48:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ddb6114085d29f6feadc52b85130bb556649dad85820b38ee5a001c7aaf15842`  
		Last Modified: Sat, 01 Feb 2020 18:02:53 GMT  
		Size: 53.8 MB (53804304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
