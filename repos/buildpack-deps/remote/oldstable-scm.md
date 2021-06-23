## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:b5cb0d8f1ade0d4700d1c32662182bae10dd7b76e61d34b03748d8331675f885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull buildpack-deps@sha256:d42f37cfb8b6430e2cea3bff684b3e41b8e550cbde62a3fece3f381faaab3616
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106587738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7990de463764afb055b51ca1dfe7e40e769584f3d3c8ef38ab567771995f7ff1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:01:01 GMT
ADD file:f9987935a0f0d3057590a5bfe45c9d8aefa9e442c57db487f8b67540669b57d4 in / 
# Wed, 12 May 2021 01:01:05 GMT
CMD ["bash"]
# Thu, 27 May 2021 19:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 19:58:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 19:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6665c6433be6a95f09c5848a9d88c4bccf7d8279967ab968e389649b956be87`  
		Last Modified: Wed, 12 May 2021 01:12:52 GMT  
		Size: 44.1 MB (44092037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a7c7a749b85354a55600afeec12c0382c7244e869193efc1da9ea0f6c35fa`  
		Last Modified: Thu, 27 May 2021 20:08:34 GMT  
		Size: 10.4 MB (10350521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca2a8c0443c6cb255beda69ddacb146aa3c727a7774c67ad0d5727b80712028`  
		Last Modified: Thu, 27 May 2021 20:08:32 GMT  
		Size: 4.2 MB (4161453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1560d5b29ea169ffd0ee927d7d52334266c7bf0c243e32c9219f48ee38c1c19`  
		Last Modified: Thu, 27 May 2021 20:09:02 GMT  
		Size: 48.0 MB (47983727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4f68b8204580122e98f9e53f24c2a0cc29115676e80c744010988c15abbbb950
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102118252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f868c78a0e4a6805c18e6113f33f6ad8f6a7454c59ba297a6bcbad3722ef96ba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:11:51 GMT
ADD file:81cfd4e746bdfcc19847240b77012487652be22dbd5741ccb2485a4207f2b73f in / 
# Wed, 12 May 2021 01:11:56 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:45:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:46:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55b9a6b6b2552c5b2eac0a316e75a7bc18092819ee25c4f1d4d54700bcc1d3dc`  
		Last Modified: Wed, 12 May 2021 01:21:23 GMT  
		Size: 42.1 MB (42120307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba756a0ca8996787a145d62543ecf7cec523a638705be132f442d2013655149`  
		Last Modified: Thu, 27 May 2021 01:06:39 GMT  
		Size: 10.0 MB (9950803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61945aef6a8fee06fbe4dccead7cbad9da46ba174cee1eae1f813541ddb76b3`  
		Last Modified: Thu, 27 May 2021 01:06:38 GMT  
		Size: 3.9 MB (3921169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad0df1f1fa0c631401a3729be99927a3afcaa022e4dd89e0acc026805d6fd2d`  
		Last Modified: Thu, 27 May 2021 01:07:07 GMT  
		Size: 46.1 MB (46125973 bytes)  
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
