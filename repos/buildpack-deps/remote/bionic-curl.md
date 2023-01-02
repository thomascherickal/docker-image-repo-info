## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:e8f5ef48c7cc40411875bd14207d6ef90357f22c2283a23be56fb249f30c89cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7754582c1b9ccb6d337821fb0b1519fb9e53c3718e38c633cbfee6eb9e0e3b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36355405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456e15cabe7032a5754df53651bfa0d0977c7a3beeb577ae95887307b5e5279b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:11 GMT
ADD file:3c88cea17de40599dc8b8da90adc8439635066835e930f9573ec6cc856c5c096 in / 
# Fri, 09 Dec 2022 01:20:12 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:53:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fb668870d8a72b5d72a3b6d98ee626e00f9f7c29c6f4f7d3a63673d747dbffe7`  
		Last Modified: Fri, 09 Dec 2022 01:21:25 GMT  
		Size: 26.7 MB (26711459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae2fe226e32be2bdda7461072a27e452330d588e627c7410d3e0c4df49ebb7`  
		Last Modified: Fri, 09 Dec 2022 04:07:48 GMT  
		Size: 6.6 MB (6617788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d279765cf084ae227e518a350e7c71778a38e42ebb7040fbde05048ba430b66`  
		Last Modified: Fri, 09 Dec 2022 04:07:47 GMT  
		Size: 3.0 MB (3026158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:270dcd62bb5758e072d43449f37df6dfb4c30b5a215d120de2995347bd6adac9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30571311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709772ab80ecddf3832c112c4ce364153036a026051e3cf3c219c02c8d8a17ba`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:03 GMT
ADD file:cf683f390855e268ca2930c28392497f485654dafd62a650da823efcef1745da in / 
# Fri, 09 Dec 2022 01:36:03 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:33:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:33:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:29b9b245ab7f1e4048f102d2f379b2ccf1f79e34f23dbf1ee57610f0ec70a4b4`  
		Last Modified: Fri, 09 Dec 2022 01:38:23 GMT  
		Size: 22.3 MB (22305207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8999222233ef373db15e3b18cfbd5729ea9165f86b03b197c2b9653d10ad60cb`  
		Last Modified: Fri, 09 Dec 2022 02:53:39 GMT  
		Size: 5.7 MB (5680158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbada3f9c5cad5c160f7d50062ce28dbb088541f9145ee0ded5d455697032f20`  
		Last Modified: Fri, 09 Dec 2022 02:53:38 GMT  
		Size: 2.6 MB (2585946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:366ccccbe0847130898cc613cb765fe81697fce4515d69f1d97b6d23c8d09047
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32580070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7bec01d161e5f7ed4a37e463f6fde9e9f38e7b67c219cf7126d830bfda2e35a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:26:21 GMT
ADD file:0acff7d2bb94db4847afdf5ab7b4385732c0a38fd82b0057ce0459f2b5d04042 in / 
# Mon, 02 Jan 2023 18:26:21 GMT
CMD ["bash"]
# Mon, 02 Jan 2023 18:47:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Jan 2023 18:47:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c347df5277017bf1ab15f258630e012d44bb79c509675d9464f96570668efab0`  
		Last Modified: Mon, 02 Jan 2023 18:27:02 GMT  
		Size: 23.7 MB (23735210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57589a61e75b6fd9c40b958bcd242697d3bd9c18d4e46b2ab119920727081ae`  
		Last Modified: Mon, 02 Jan 2023 18:57:37 GMT  
		Size: 6.1 MB (6054448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fe4f939a742980b846ab4256c36fd2e683a0409f5c4655aced05555c4bf9ee`  
		Last Modified: Mon, 02 Jan 2023 18:57:37 GMT  
		Size: 2.8 MB (2790412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1c967b86edc86a6f37019460490e7787e99fa7aa209ee7f679770ecb0faaefc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37109590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7670feca3b83449f297a04c491c56f43fc850975346f5576a22190b008bd581`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 02 Jan 2023 18:00:42 GMT
ADD file:dc76519390168deb6f9bb6052d08c6e7840908a831276d99bb19c6c245f8517b in / 
# Mon, 02 Jan 2023 18:00:43 GMT
CMD ["bash"]
# Mon, 02 Jan 2023 18:22:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Jan 2023 18:23:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1b284dbae22f155bfee2a25073c97c9758e66aa7129a455cb533d8e2cbc873f9`  
		Last Modified: Mon, 02 Jan 2023 18:01:17 GMT  
		Size: 27.2 MB (27165399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd588f5ab18433db51d33fb54b32dbf18f5af8fb4dbd30b3407f93e99ff057a9`  
		Last Modified: Mon, 02 Jan 2023 18:28:46 GMT  
		Size: 6.9 MB (6902109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bf514bf8c4c2f919659a2f58d292672576181c783d997d3caa71f5818bb613`  
		Last Modified: Mon, 02 Jan 2023 18:28:45 GMT  
		Size: 3.0 MB (3042082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e93b15bbb557dda17b3f275619b695955e6b693320c69c387927ded2d2a4559c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41219125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df44988a08ebd3b332219230f05fdc493c5dd68a07d4b6000b593aef1c2a27f8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:15 GMT
ADD file:05ec256cb279f6d94111b2413d31c85c4e1ff1365bce34d2fc4aa2788885fa06 in / 
# Fri, 09 Dec 2022 01:27:17 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:20:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:20:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:29d5a8bf9800ea1d873fe104fc2b0b6d4efed1269ce0f9a80e4d65e96d3246e2`  
		Last Modified: Fri, 09 Dec 2022 01:29:45 GMT  
		Size: 30.4 MB (30442475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385b911dcd17dcd21857c45f1580921dc1ef7a6bfbe01898fef3a628772fa8dc`  
		Last Modified: Fri, 09 Dec 2022 03:50:15 GMT  
		Size: 7.0 MB (7036031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e182844a761cb72bff2c8199230ea0379f9a69184d085e6a53f7c24e9f815c`  
		Last Modified: Fri, 09 Dec 2022 03:50:14 GMT  
		Size: 3.7 MB (3740619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b29db8a61ab86d51663ec941b1e15d98d03821e100704d03885af7864603f507
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34656891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3617e881f76693b6a2209d9f927759784d33b757626ba5bc014c705b6b8c88f1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:52:21 GMT
ADD file:c2fcdae7883d865c232dfc26d514c111189f6940ba74273c78067624cd02c962 in / 
# Fri, 09 Dec 2022 01:52:24 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:35:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:36:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3fb013d46f2fda49d6c671f39f55c3330f927a4c55ae7e5096daf0a638dc38ec`  
		Last Modified: Fri, 09 Dec 2022 01:54:45 GMT  
		Size: 25.4 MB (25371298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d3308c646e5c998e89d5d8adcbf8cd509d32cca837db45b2d5c82b50e285a7`  
		Last Modified: Fri, 09 Dec 2022 03:54:11 GMT  
		Size: 6.3 MB (6308863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abb84decd56d62b11ef05936ef3afa942b0ac06afa5119cbb7104d11e4f6934`  
		Last Modified: Fri, 09 Dec 2022 03:54:11 GMT  
		Size: 3.0 MB (2976730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
