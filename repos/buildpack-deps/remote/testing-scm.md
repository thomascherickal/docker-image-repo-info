## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:67b479b2bb657117dc792c545e02de64b67cb196af0dbd5868007f3fe79cb424
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

### `buildpack-deps:testing-scm` - linux; amd64

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

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b0faca890ecf5b683240c2dbfc86375d4ca3255996d4b2d5e7da11d7b5a7b6a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119167889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beaa74ea5de80ed27c5cee446c4aca9e9417a30a15c28ec3e5b10aabfe8a6dd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:49:39 GMT
ADD file:b4c3e18bbf2b51c4f777d44bb8ef76a6fd78e8e9e057ffeb792fa8e041d3b40d in / 
# Sat, 01 Feb 2020 16:49:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:18:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:18:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:19:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1758f12059aa2a6d57dcc649233827a3b49cc528e7868081891f2a12944a479b`  
		Last Modified: Sat, 01 Feb 2020 16:56:07 GMT  
		Size: 49.5 MB (49485065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4449c159b35252b02eefe1b4989bc90d10d35fd6d17600ae5d662ba279c259ad`  
		Last Modified: Sat, 01 Feb 2020 17:43:56 GMT  
		Size: 7.5 MB (7494059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a6070fc56cb0dfa20ffac6472ce9dc9a8aead19638f495a62bff5206bf6ec7`  
		Last Modified: Sat, 01 Feb 2020 17:43:56 GMT  
		Size: 10.0 MB (9969002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5ef05714eb441ecaca79d450dfa2444ca3fe859d6c1080d660e208a78633f7`  
		Last Modified: Sat, 01 Feb 2020 17:44:18 GMT  
		Size: 52.2 MB (52219763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

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

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1ad465ece6b0be36a2aceb609195daa2abb6d9f5447f13d909224a17ac1c45ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123213873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0220f84d7210a24cbebda84f75a2a4f9eeaf8c7119f4ddc7a3c826283305d28b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:40:13 GMT
ADD file:485f0f88566199683d3683f547dbd33fa9cb4897121b104dd7c852162fa06cf7 in / 
# Sat, 01 Feb 2020 16:40:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:14:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:15:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f625aea7552a55d9aac253c9834ea6e645ae1e9d641ccec7e167585699e5d1b3`  
		Last Modified: Sat, 01 Feb 2020 16:45:20 GMT  
		Size: 50.5 MB (50453025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2bd511eb67667a40782667bc3dd7eb41f584de23c5a106085d2a1db980df9`  
		Last Modified: Sat, 01 Feb 2020 17:33:39 GMT  
		Size: 7.8 MB (7792989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f4fcee540ca05f3c8904722b70f13e10600fced1073a2612d04d995a93d210`  
		Last Modified: Sat, 01 Feb 2020 17:33:39 GMT  
		Size: 10.2 MB (10245802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5c01ce24c138f20821dc546f2dafea1d7baf1be4863e4de4f1957f18bb1577`  
		Last Modified: Sat, 01 Feb 2020 17:34:01 GMT  
		Size: 54.7 MB (54722057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

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

### `buildpack-deps:testing-scm` - linux; ppc64le

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

### `buildpack-deps:testing-scm` - linux; s390x

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
