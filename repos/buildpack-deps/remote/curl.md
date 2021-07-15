## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:0db82fd3e508b20a887ed972fb446ad17928ec4a7dc2b3d42bf8e25daee68ee5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9019c657e4566c337a72b88646b3e29cddb6267fbff96337b7035e6c986dee2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68265869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0eb972ca145363dd7a1fcdaa5708a2d86e3f7abf6ef4a832da1f20d9f214e1c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:316e8323241e407a1058ac38040373b3d7ad8f3c9884144e53136cc13e78beac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65217841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26bcf6551305dda94eadba6183860b74c8b8c3151690704fced19a1c10ab2a83`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:38 GMT
ADD file:cbb86580a65f84ec39691b126a21ef374bc4f2f2fe5c27979134aa940d6326f6 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:39:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3b0b1347a8a3d1156e417fffc79192d014d9cc985fa5e55a49cf67c21e7a81da`  
		Last Modified: Wed, 23 Jun 2021 00:00:57 GMT  
		Size: 48.2 MB (48153698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516d9fa44d74100e5f41bad5b510ea489670072286500cb3e7ec282353be3fd6`  
		Last Modified: Wed, 23 Jun 2021 05:57:15 GMT  
		Size: 7.4 MB (7376607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0bd36c0872a5d6227f9c9a854165764990cd8c08f66f8fb948836745f04edb`  
		Last Modified: Wed, 23 Jun 2021 05:57:16 GMT  
		Size: 9.7 MB (9687536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d6a5ba2831645a58a411d6bb3df8d2df660b37a8a4a8d0a4855d313c4c5581ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62385513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680c1305b1a311761bb18b91e87c15b9b0b8ca437702c276d0a346e92b44971e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:01 GMT
ADD file:3edc1a2322b55593b3cd8e935ca6d837e7618bcaaab27a09c9822728f8272ce0 in / 
# Wed, 23 Jun 2021 00:20:02 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:46:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a3ac2852d9d20585eb4d19973a45b69522d16832456ea5b52f0298b2937afc09`  
		Last Modified: Wed, 23 Jun 2021 00:31:04 GMT  
		Size: 45.9 MB (45917482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d59952ec0a1da3155a9d9a84f07fc99163c3b5429cae2d6d37e9de664191d9d`  
		Last Modified: Wed, 23 Jun 2021 06:18:36 GMT  
		Size: 7.1 MB (7124226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac8017b9330d1a833e533de62b0525c9033b03c74f0d5c3b28b478231b03803`  
		Last Modified: Wed, 23 Jun 2021 06:18:37 GMT  
		Size: 9.3 MB (9343805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:837220a1d60677864e23f4856c397c131fb5dafe0b7862a92ede974fd8a9f119
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66900982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:859054f03e5ef4db62ed73e51bd267a3777c563f0cc66459d6839aa8515e7970`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:cdc588294a349c7cf415c95d44a5a119b04299f18e793342de2f3598dee4af40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69545424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe906c9e35af47e67e96846160e6b06def38337a6982f5e3bc9fa4a980d8146`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:18 GMT
ADD file:e69bc1dee51190c812075d4b4e8ba1e67f67250af9f2ddbaecaf2c9316a07bbd in / 
# Tue, 22 Jun 2021 23:39:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c4109247a8f9a72ed1435270480f72d6db8d6f038c6941d86a94f4dd0be8f789`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 51.2 MB (51207098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823a83541e8a9ed59943f9915ac65a73f57137e829772a16bc0bca5031a8cc07`  
		Last Modified: Wed, 23 Jun 2021 00:17:58 GMT  
		Size: 8.0 MB (7998521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7455379cfe2e69e9290d3b103e5889bee3e1c03187bb9e2a454325fd6a7f1a`  
		Last Modified: Wed, 23 Jun 2021 00:17:58 GMT  
		Size: 10.3 MB (10339805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:f1552cffe548ecb2d77e3e1988443dc967bbc547754bffd84ee87b7c715e4e33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d47563b5f23c3a60d650a24e54817028c7372fbaafe2974e74598b358bffa6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:06 GMT
ADD file:4673ab387e5a746227250295a00343ac2d03d6aafdc28d019a9bdf26bb97c8c8 in / 
# Wed, 23 Jun 2021 00:09:07 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:42:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:42:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e3f0127f2925aa298e3074daa756fb98cf945e5aa11c7dd3cb6d66cc3ba2c7ac`  
		Last Modified: Wed, 23 Jun 2021 00:15:06 GMT  
		Size: 49.1 MB (49080336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92573df8c3dcb8e821060f2830e027ebc52f7da05600cbb49cfdbb39aedcce5e`  
		Last Modified: Wed, 23 Jun 2021 00:53:52 GMT  
		Size: 7.3 MB (7252466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f80da49549480363cca077bae713c30796f17d3a33620cdfca3a75e0cd160`  
		Last Modified: Wed, 23 Jun 2021 00:53:53 GMT  
		Size: 10.0 MB (10016316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:58a15931fc86ec259f00476fe38138ed88aec8183132788679e72a24f6eb4254
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73182096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e009315ff55d93c486b0ea54231698f7a334172893174db0278241f08172a2bd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 15:57:37 GMT
ADD file:b73f8d66b8be6103349949991124c7d82e38589b2db6212e920cb3b6d5ceefef in / 
# Fri, 09 Jul 2021 15:57:40 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 06:21:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 06:22:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:83f72610ec8bc58c0c3a70f0bdf9d866e8d0156845a9aa24bc0ed2fdaf0fd8b4`  
		Last Modified: Wed, 23 Jun 2021 00:36:35 GMT  
		Size: 54.2 MB (54182463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ba02bc6289674c1f1edb2ead79c9223d07b7bbb36fbf1ad389ee06ea3cb2fa`  
		Last Modified: Sat, 10 Jul 2021 07:06:15 GMT  
		Size: 8.3 MB (8271883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6dd9fe5e0862c666475fcf95f93e2e378b2463bf5bc4da89adc0d524db7b85`  
		Last Modified: Sat, 10 Jul 2021 07:06:15 GMT  
		Size: 10.7 MB (10727750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c9498d5c6327e3d16faf01a548371287dfaec142b937a303a25e5e2f9b27bb29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66287603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22ebf8e317fba295ee8d1cc8342849b7429d8a021fe0b28a349c4e39889ddcb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:14 GMT
ADD file:b935574081a3fbceb534880a35e5245e10c52a3b9d70224811e221b4c6254cfe in / 
# Fri, 09 Jul 2021 02:50:15 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:43:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:43:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2b8d113de06cefaa0768df3e10da0c3b8272e15922e18ea75b0bb4dee23b551d`  
		Last Modified: Tue, 22 Jun 2021 23:45:28 GMT  
		Size: 49.0 MB (49003924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709081180ba661cb2b844502980f018e41ba05c9f731d82ea24c0854129bb083`  
		Last Modified: Fri, 09 Jul 2021 03:51:27 GMT  
		Size: 7.4 MB (7400478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d96fb2bd130de1d62dc0a655e6b1361ea22cca1a97e879d4e80a6b8aa5f9cc`  
		Last Modified: Fri, 09 Jul 2021 03:51:27 GMT  
		Size: 9.9 MB (9883201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
