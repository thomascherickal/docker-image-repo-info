## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:8dabe4df1318a2cc7d615d7ba3fb9d06b128843d1dcdbf41fe3849c438e2f1db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d7fa12cd3d76b3435a5aaa6844f5f3d74b1a250a230c27e9f38f24bb12411320
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110778527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705227197d8ce8b2433d1cb46cda0062cf46fa708a56e9760238dfe9e951cc07`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:59 GMT
ADD file:899a3c031d50263e5fce253aef92e05aec77f14ec3c38a37f08414e4c9b358f2 in / 
# Wed, 23 Jun 2021 00:22:00 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:56:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:199ebcd83264652823564822c7ef553db971042e35d7f347f66ea8a60a480545`  
		Last Modified: Wed, 23 Jun 2021 00:28:01 GMT  
		Size: 45.4 MB (45379993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbb155879c013b8bb809e63f37f6dae34e890ec41f5a108d57f0958ca7365bf`  
		Last Modified: Wed, 23 Jun 2021 01:04:33 GMT  
		Size: 11.3 MB (11294536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c194bbaa3d8bb7beb2bbbf9e74fc0fa7b6354f836402482f35b408c9163c5792`  
		Last Modified: Wed, 23 Jun 2021 01:04:32 GMT  
		Size: 4.3 MB (4342418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6154ac87d7f3d5133865f50f67a37cc0687318bb4f422ba4f2d65057e9c266fd`  
		Last Modified: Wed, 23 Jun 2021 01:04:53 GMT  
		Size: 49.8 MB (49761580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4907ff8c824bae7e82e3df48bc642ba0c3cfb51f8c33902215ab78841d798ba1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106585313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f309324066d95a8e915c94797ea3b07f8b19d8f1794b81bbc6b6479bc6e057ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:52:47 GMT
ADD file:ac76479423dbb474270e853128fccece010f64fd8b2cb114c2a35b3da5b74756 in / 
# Tue, 22 Jun 2021 23:52:49 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:47:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:47:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:48:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a89c1f87f7fbe989370a717a85446a7926b68d3e20e9344a5078c8c4bb39cfff`  
		Last Modified: Wed, 23 Jun 2021 00:06:22 GMT  
		Size: 44.1 MB (44092051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce999550135ba50d963d58322e2d09a3a084cd766ed8449c118be071ef8ad7cb`  
		Last Modified: Wed, 23 Jun 2021 06:03:50 GMT  
		Size: 10.4 MB (10350647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe4d0fe9f0a7e8f148770529b1c6f3051f91b6d2af3d3fc896fcda1dd4041b1`  
		Last Modified: Wed, 23 Jun 2021 06:03:47 GMT  
		Size: 4.2 MB (4161509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b652b05d87b08a7bb0c350aed15b39a5abc21d3129d0b1e4169061bb7661b4e`  
		Last Modified: Wed, 23 Jun 2021 06:04:40 GMT  
		Size: 48.0 MB (47981106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8d3150615bfc388d914effa98ecfbde05d91cdc288039602956ad321213facf4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102117964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337d4a0b5c23a5872d4728b110ea65684e08fbaed63bbae14ca0d09ad8bec353`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:06 GMT
ADD file:8c289b4c3c40ee076e3b3563f38ccd72dee8b2ee3122170cf1bdd417ae9e03c0 in / 
# Wed, 23 Jun 2021 00:23:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:53:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f34e8839b40d84b70d62e2c8a6909422dad9688919bf387ad4a092d38ab62f`  
		Last Modified: Wed, 23 Jun 2021 00:36:08 GMT  
		Size: 42.1 MB (42119988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327954c584e8a66a22440b9a731a29ecccc047aa5f3477d6191e1c7167a37503`  
		Last Modified: Wed, 23 Jun 2021 06:24:47 GMT  
		Size: 10.0 MB (9950929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7274a619e45e9e714e599f6ae62b529f504ec947a07a58908ad99c464907420`  
		Last Modified: Wed, 23 Jun 2021 06:24:44 GMT  
		Size: 3.9 MB (3921297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9912efc947692ebde57dca8997537ddf30def320f8ba3667b58994d42617114`  
		Last Modified: Wed, 23 Jun 2021 06:25:35 GMT  
		Size: 46.1 MB (46125750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:57a73f9324fc6907fb0ba178a4d20d991a9398bef205c56c7f67f26c1e2fc2de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105221355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c3560ffd72f476ceb68be75ab42a324c0475441f55df7a2d0e8b6823a9eac93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:55 GMT
ADD file:02285d0bd3ea996a7ebbe069a83e508701cbaf14f53fdeaa123775acd7e0537f in / 
# Tue, 22 Jun 2021 23:50:56 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:27:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0789e4a342a11c7c57a241829a41af53fbd194e6dede60c6d6f63d69e403b2cd`  
		Last Modified: Tue, 22 Jun 2021 23:57:52 GMT  
		Size: 43.2 MB (43177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd2ed69368e8a7d296f1c91060e897753bed4a79ab68ed47c544e1f4d6fadcd`  
		Last Modified: Wed, 23 Jun 2021 00:35:58 GMT  
		Size: 10.2 MB (10214577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c76e514669ff971481e0d19dc0581f90d72eab2d0e117a5761ae016e14f213`  
		Last Modified: Wed, 23 Jun 2021 00:35:57 GMT  
		Size: 4.1 MB (4096534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa19114dc4cc7157e619bb778418a2fadbc86acafe444fd2066e1412d2a7fb8`  
		Last Modified: Wed, 23 Jun 2021 00:36:18 GMT  
		Size: 47.7 MB (47732823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f09de8dbbab2ac2b40949d008093956df79407ebec4fb445d314b5c3bebe18e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113279940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb512ed2af229734466a3ae3f07aa0ab0e92232d1466d2581d5a75a011daf1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:41:10 GMT
ADD file:80feef1b55f2f1e39986ac669152a7a209e2fa5a097a8dfa16ca7e1118159830 in / 
# Tue, 22 Jun 2021 23:41:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:12:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:13:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3497549dbcdd02a0f25068f37e6950ad5b608b1791d0c79236abdfe13b8e3f02`  
		Last Modified: Tue, 22 Jun 2021 23:49:21 GMT  
		Size: 46.1 MB (46096990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908bab0e9cd5e81a3e8bb8d6a886f1f7d5058bed177f7d72aaa41cbc1be07c78`  
		Last Modified: Wed, 23 Jun 2021 00:21:09 GMT  
		Size: 11.4 MB (11352293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d81c9417ef64635e730e26eed1f82f02fa869f476770ef658a95fddfc192319`  
		Last Modified: Wed, 23 Jun 2021 00:21:07 GMT  
		Size: 4.6 MB (4564980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec9dd8c9a561c924b995bbee8e6986503521fd6ce2ce66ce18c154371379e11`  
		Last Modified: Wed, 23 Jun 2021 00:21:34 GMT  
		Size: 51.3 MB (51265677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
