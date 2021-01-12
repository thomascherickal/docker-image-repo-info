## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:959425bb5c46a3d83ba8a7a5d7dcb8bc181f2197016fd3d9348db781722d6456
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1a9f55f71143aca2dd01ab0a365e469c3203543ff5194fb519ae5183e80af5b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72602212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60eb182876824d03f6581e048ad13b41a5f8350427642eb5671f68d4e499f3be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:34:16 GMT
ADD file:f1c9279b9eb3b88b40c4958324519afa81185c0383ed51d5138ebf2a0eff6d7e in / 
# Tue, 12 Jan 2021 00:34:17 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:59:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:abc50f4e181143f18afce1a5282914e00abd896a798d96f7514e728b30f0988d`  
		Last Modified: Tue, 12 Jan 2021 00:41:42 GMT  
		Size: 56.8 MB (56800959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e331862b1a60a0f0273b0162c4d7c2b7bbe7a7b631e4a7847799daa4d3d614ac`  
		Last Modified: Tue, 12 Jan 2021 04:07:28 GMT  
		Size: 5.2 MB (5151057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621cee81c84693094bc652651e3d6789dd350ca0bd2dab361e7677761ef3a02`  
		Last Modified: Tue, 12 Jan 2021 04:07:29 GMT  
		Size: 10.7 MB (10650196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:66ea4829231b164eb0d8c38929457ee31c35ec9c8a985f42afcd6f3fcf7d985a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69759828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c75ea0a0bc7d4479d9fde38fb10753d5f17b1fa0f7eaf7096a004ea439a1b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:53:57 GMT
ADD file:7c196731dd997fe0c289ed02eba35ecfe200559ab33bcd6e863f39d8dd0ea362 in / 
# Tue, 12 Jan 2021 00:53:59 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:32:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:33:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8703e0802b99292f132d58e67ad879ab0ffa44370ae81a8ca7a93ee05c332d4d`  
		Last Modified: Tue, 12 Jan 2021 01:03:20 GMT  
		Size: 54.4 MB (54362040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2920a5dce5819aaefba9b42acf5eecc9bf6a9cece8f1115be0561cd7604d55`  
		Last Modified: Tue, 12 Jan 2021 01:45:30 GMT  
		Size: 5.1 MB (5061367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ad854c9d78348debd410e2b83d72c46ebbefeabc275c2a9fa7877161420d56`  
		Last Modified: Tue, 12 Jan 2021 01:45:32 GMT  
		Size: 10.3 MB (10336421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e356e5ac5188d78a70152f60bd21544b0644f70f6015bfe55cc9e61ed2b8c6a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66799885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:726f975af02037fc20209897bada81c0761bc91cb1dc67aa9f810db4a80523e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:03:45 GMT
ADD file:a459be4601ccf608a415f6ce53ea885edd1a9a10ba1205f3e8493e277e6a7faf in / 
# Tue, 12 Jan 2021 00:03:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:17:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:18:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2fdfe7e087b5c823888d02320fcca90d4debb7a7d0ead6a978abb2de6acbbc00`  
		Last Modified: Tue, 12 Jan 2021 00:13:47 GMT  
		Size: 51.9 MB (51902171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0592e7529a748d8d0e52ef640addc32dcea717609f5c656e4399e87bdd4d9db`  
		Last Modified: Tue, 12 Jan 2021 01:31:29 GMT  
		Size: 4.9 MB (4921500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeb968aa1e6a404fcd0a89cbc65878f592c4c4067725853712ca4d00c1669ce`  
		Last Modified: Tue, 12 Jan 2021 01:31:31 GMT  
		Size: 10.0 MB (9976214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:82856d2e3fc65017f1ce3081d0afc61f78a1c72f10e1443febed08cf3f8b66f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71333978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:017a27734a612b9e623d0d5b0b809b87a033a3030a7a92f734d6f17b98c6f28b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:27 GMT
ADD file:ba9ce45e2c6743713798982615c806de6db6d8fd9a0d8734c8a69d80f3959eb6 in / 
# Tue, 12 Jan 2021 00:42:35 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:27:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:27:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:01dba80e9024f3ac734ae74a14f2997ea67918b4de57aef778ed839a508baab1`  
		Last Modified: Tue, 12 Jan 2021 00:53:15 GMT  
		Size: 55.5 MB (55537816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8417d785c975de855b94a5c17e92b69107a02149bbd61ac1b6d1355d80b32549`  
		Last Modified: Tue, 12 Jan 2021 01:40:11 GMT  
		Size: 5.1 MB (5140360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34511ce04354db34bda0eb613bcb4990a4e262fe16307861b007423a0033c44`  
		Last Modified: Tue, 12 Jan 2021 01:40:13 GMT  
		Size: 10.7 MB (10655802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:53d8db8895fe8bd5c0d968f5867a36c1e0ee1d6bd27c4ee5e2b53e4ea560f9be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74252644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7969c1664f3825e07a3bc29a1dcb64e68d09b376b371ebbb0f0f37d700f353`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:09 GMT
ADD file:f368e139210fa607baf12a595022c06210c9840e9f988eed126d02b3ed2abafb in / 
# Tue, 12 Jan 2021 00:41:09 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:20:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:21:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e50ef36c9f800462aaf97a2c77ececa8643ebfa28c18c3c5df44156f678ce9de`  
		Last Modified: Tue, 12 Jan 2021 00:49:10 GMT  
		Size: 57.9 MB (57940505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971fb6fb93c9113f602d7475b69f429dd8d1c0e65ab51621f1f1b5d26e20d9f`  
		Last Modified: Tue, 12 Jan 2021 03:33:00 GMT  
		Size: 5.3 MB (5279224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade23daaaac90ab6a6ce682aae0cac5066fc7dacb15fba678df545ba532d7fb`  
		Last Modified: Tue, 12 Jan 2021 03:33:01 GMT  
		Size: 11.0 MB (11032915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:90d9ec6269ba7bbe838cebf1a3f20e4dfce6db2cde4d238c2c683bf1a172c35b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70819358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ee50d214753a082da0974f08ca77722e5af2f3d13867b8ee37dc17dcb6f2fae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 01:16:48 GMT
ADD file:7bfb9d47fcd2b6a553e5be3b702d34f192cd8798dd3982fc6e6e77479f0affdc in / 
# Tue, 12 Jan 2021 01:16:49 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:54:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:24a4375dbae3deddd016bd6d4372d219ba5fe4102ce643c06dd57677bc882654`  
		Last Modified: Tue, 12 Jan 2021 01:24:08 GMT  
		Size: 55.0 MB (55046139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1447ce8a926cf7692ae55e3f2edb9925e5b11be684c7fd68fe2a385a5b812880`  
		Last Modified: Tue, 12 Jan 2021 02:05:46 GMT  
		Size: 5.1 MB (5114938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfd08658a76a7d3cedb6b4760f760c0ce830104bb77dbffd92228d4d0448730`  
		Last Modified: Tue, 12 Jan 2021 02:05:49 GMT  
		Size: 10.7 MB (10658281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:da824faabb1cf2483f9dbad980dddf2f52929401bd4acbec3c9d00f8ba02bbf7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77871932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601396709b1c2887e79a72d7aae4ba82e979288ce9e936a41faffeda3a37170f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:40 GMT
ADD file:f289d6dea557bc0563fd9221c4857a56c56bb52d981a3ec90ade2f1b76980794 in / 
# Tue, 12 Jan 2021 00:25:56 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:22:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:594e638823d3ce0bbedac4d1aebea00f91d28a98d7b98ca680fd90e4c0fc8850`  
		Last Modified: Tue, 12 Jan 2021 00:34:46 GMT  
		Size: 61.0 MB (61048727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a59148553af7496dfbc29a5704e94338ac15ab898a646dcbab32076a5f00f3`  
		Last Modified: Tue, 12 Jan 2021 02:40:41 GMT  
		Size: 5.4 MB (5400394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45a065f7b5587bec16714bce093a4075fb92b291238fee1bae7d383a16a4052`  
		Last Modified: Tue, 12 Jan 2021 02:40:42 GMT  
		Size: 11.4 MB (11422811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a35eec5fd9cedc0345232d51b60fad328080156877082b248e3db2ba397686f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70700646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2f620bf76683d87710b1ac4b7a3207579a6d4e642427391a6ea25e73468d419`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:42:33 GMT
ADD file:168fa93b7a5e386f9127b8b0d3ef48b98f82ba06ff1d48ac529b03d704687af9 in / 
# Tue, 12 Jan 2021 00:42:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:12:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c7a519e99fa2bc8473c6755b8e9be0f1d685a3d42426bbd0d3e942b5d1f9a4e8`  
		Last Modified: Tue, 12 Jan 2021 00:54:49 GMT  
		Size: 55.0 MB (55038475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c303cc6ccc4ed36f7947903ef4cd9e4d9325b5495c5019ac8262fbe63bd0acf6`  
		Last Modified: Tue, 12 Jan 2021 02:25:30 GMT  
		Size: 5.1 MB (5135101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2547d9300a261d759832bce2972dd571e9149f705eea6a0b45574d2e535745e7`  
		Last Modified: Tue, 12 Jan 2021 02:25:31 GMT  
		Size: 10.5 MB (10527070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
