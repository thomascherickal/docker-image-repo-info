## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:36d53aa194ac5a055f31423d9d0227739b1ff7dcaf72e500306cdda89ac9016e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:00d382010f16ca4dd469786ff2e4f7ce37628594436034481315aa685c639495
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36373306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9a57b4e9734f594a5e14639d46ae3178c0efa501540ed71de7792581b996af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:25:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:26:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce443e20fc86732c10960851f26800e6cebf13458f8dcf0cdddaaab061c3599`  
		Last Modified: Tue, 13 Jul 2021 23:44:31 GMT  
		Size: 6.6 MB (6644641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f37762e578acbec391decc8fb89c06ef4df6bec5669eabe1333e533deafc72`  
		Last Modified: Tue, 13 Jul 2021 23:44:30 GMT  
		Size: 3.0 MB (3022520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:61fb3fbcbd1d585dfcb0e1e7736910475595174ba84e639fcdcd3287b528f28f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30603254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0f8d7636e62cf8f283a8c1d0a020446a8cd1f092fc94df6ecfe38a6a930947`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:48:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:48:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a381c1b56daf40bf0a1cb605f054f5f78996d62b7fd03202bfca93d60105a`  
		Last Modified: Wed, 14 Jul 2021 02:13:52 GMT  
		Size: 5.7 MB (5714793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ab2aab067e36310e0780e1cc2b823b8a20a57e2ea500e79253cf059a4389f1`  
		Last Modified: Wed, 14 Jul 2021 02:13:49 GMT  
		Size: 2.6 MB (2584388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:448e829dab2190d069623728c1f0c5fb4f1c67a6cec747f682de9642ce774af9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32598355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4f6b20c985b74f83b24eb07c5a27a8ad36f65df45f0154c30719325616555a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:49:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:50:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dd214c2ad05851ec94a967ce88d916213c618be25a5c78530c7c7fdc3bb7ce`  
		Last Modified: Wed, 14 Jul 2021 00:00:36 GMT  
		Size: 6.1 MB (6085843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157d01128028baa4cf94da75d0ed8d9f006b6cfb22d1991abcf7d00ea5b8d5b8`  
		Last Modified: Wed, 14 Jul 2021 00:00:35 GMT  
		Size: 2.8 MB (2783014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c3a1a408cfc2d11deae49b0405a72694a599d652f9a3ccb5962385f1b25543a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37338345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da5b6054931839f8e08914e10dafbd0ceedbddc97b4158736d9c1e78a92bb948`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:39:15 GMT
ADD file:2478887c0caae58ac755f71306211decbf5e69b832b9939974a93743e5c440f5 in / 
# Tue, 13 Jul 2021 22:39:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:57:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:57:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4c0067b0d84ac31443135f34e6bf8eacb1e1da0b388d042fbdd498858738047f`  
		Last Modified: Tue, 13 Jul 2021 22:40:10 GMT  
		Size: 27.2 MB (27153547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dd8cf59f9fe8a2a2d104b0a25d5cabf172b2865b6dc589e1a9ef6205f67329`  
		Last Modified: Tue, 13 Jul 2021 23:03:59 GMT  
		Size: 6.9 MB (6932625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c918e66b3fffa8e551ce0f942e109f82f3ff19d2a5ac43d0a3773c73a4281d5c`  
		Last Modified: Tue, 13 Jul 2021 23:03:58 GMT  
		Size: 3.3 MB (3252173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d6aefbe2c3f1be43baefdc05d2074388aac5698e03c976914116a3a775c8a3ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41201786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d3823ef25def7e22233856b34afe60700dc4b15e4891ff3684d57f7f5f1636`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Sat, 26 Jun 2021 00:02:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Jun 2021 00:05:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d73831cbe93544dd7ead7e80ce635c923ba099ca28e8498bc8302c24229bc6`  
		Last Modified: Sat, 26 Jun 2021 02:06:46 GMT  
		Size: 7.1 MB (7056533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c741d7670ab7c36401f5b1db224a1a23deaa34ae455d260a486120619cca07`  
		Last Modified: Sat, 26 Jun 2021 02:06:38 GMT  
		Size: 3.7 MB (3719897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a3f8b2b3b6be1ebc33d224c21996a521ce875365e40e38f5ff9359a4da4fd211
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34674930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e12fbc0afed5efae7a86d80a3cd6b831dd133a18b4decf8d3da37c5bc29d010`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:53:22 GMT
ADD file:9e621b1dfa735f1a89553f154f2a2a6f669ff610236d92d6ebf37d1f378d8ec0 in / 
# Tue, 13 Jul 2021 22:53:24 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3287e09e36098b10234ccc1f8db0b48e2027ca7caa353a362d65f9b017ab802e`  
		Last Modified: Tue, 13 Jul 2021 22:55:34 GMT  
		Size: 25.4 MB (25365649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50646ad897e9498b64756ff489610e121d8001f77bcd029887bff67f0280e504`  
		Last Modified: Tue, 13 Jul 2021 23:50:37 GMT  
		Size: 6.3 MB (6334299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34313261ef7b25f09c9d74570da6807db2583b78ba0bc64bd8c7cb885694dd94`  
		Last Modified: Tue, 13 Jul 2021 23:50:36 GMT  
		Size: 3.0 MB (2974982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
