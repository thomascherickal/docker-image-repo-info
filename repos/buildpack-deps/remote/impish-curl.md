## `buildpack-deps:impish-curl`

```console
$ docker pull buildpack-deps@sha256:287f27d35bce6d63f05254d1a966372a295c381d622572d83fb463f9fe888497
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c8382f9699ecc7686190ed3ba75041ec06511c7ae5be650adba6abe1a2d1e4a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38764188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f9bb8a11c0d1b625f74b36eed098e3671e1079814f7535e6fa39d4773adb19`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:01 GMT
ADD file:aad4137373f37cc2272f1632b0fa50a91b4c0c878ca72ae8de8fee51ffa2f392 in / 
# Mon, 26 Jul 2021 21:22:02 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:59:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6c8d2949e37d3f87c8d42e502aebe8d287cc56bd1f5846a5265a2124c60cb49c`  
		Last Modified: Mon, 26 Jul 2021 21:24:04 GMT  
		Size: 31.5 MB (31519889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad149f781f55b2a85f0e013b5220678d294bfdc9a113255a07b8fd871224219`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.7 MB (3692251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11936e1d3aa1eb439ea9dac0215a97aa74b71b1eabeed3965b276ff2c836d5e`  
		Last Modified: Mon, 26 Jul 2021 22:14:45 GMT  
		Size: 3.6 MB (3552048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:14cb8487c3b5aea4627a0dd934cbc37283b95eb342ad6ccc08e89753ade64ae9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34057184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f2e381f6175d4348fc21d1d747335f18ba51395951d01822be790604501efd9`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:54 GMT
ADD file:7c7c93de372cabbc1cbc45bb3618b626ecd538c81cdb8a09c63b397ac79615ca in / 
# Mon, 26 Jul 2021 22:52:55 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fa3fdc2705d50f3ad184e38a8ae9a54c70a75ef26a8f2036c5cc36454c57b49a`  
		Last Modified: Mon, 26 Jul 2021 22:57:52 GMT  
		Size: 26.9 MB (26876142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05927c7769ed8e7aa2c01453e69c9f65172154a601b0218204df2a1c260a6`  
		Last Modified: Tue, 27 Jul 2021 01:50:05 GMT  
		Size: 3.4 MB (3438752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c89b675bf7d9d2c4ea66630864775dc5879d8e56b1c77d25f08550fd9f882b`  
		Last Modified: Tue, 27 Jul 2021 01:50:04 GMT  
		Size: 3.7 MB (3742290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3b1b576e71b825c2dec9c657f0fe811c10f13092905c08a3c604e98ca3ccc887
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37167590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715e8e60a44bcfc8f6966a72d39a7d5108ad3a12aa3ceba4add63c9a62b56df2`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:49:21 GMT
ADD file:da87b88a910a756b9836fda56f61b491974f97e66462db711cde71ecfd6d28d8 in / 
# Mon, 26 Jul 2021 21:49:21 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:33:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:33:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:745e0e9e37f685fd5013fb72549992db744cf1eef9c1d0f35661c7fa8c1ebbda`  
		Last Modified: Mon, 26 Jul 2021 21:52:08 GMT  
		Size: 30.0 MB (29955429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f570b6e57585e3b4231948f69ed42c0ce2f57cce20efcc0159f7b58ca6aefd3`  
		Last Modified: Mon, 26 Jul 2021 22:43:50 GMT  
		Size: 3.7 MB (3677798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d51866b9032635ff1b654909c863aace586fd92d720475e6f21862991005d0`  
		Last Modified: Mon, 26 Jul 2021 22:43:49 GMT  
		Size: 3.5 MB (3534363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fb1ae578b0181287cdee49a1ddf90688b5634cddd1742a265064aeb8ca520596
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45497028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b814659ec88c950bcc0e38be82a3b5cbca6e6929da1fe08971ca5efa510f66`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:33 GMT
ADD file:5419572ba3a583506859cb346c0715939486d87fcc143e308557a18a73bb92b2 in / 
# Mon, 26 Jul 2021 23:13:37 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:49:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:50:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:415d912bb08e4b766d9582ddc3d0e3c55a978420909d0ce62488cfc6ddcd065d`  
		Last Modified: Mon, 26 Jul 2021 23:17:00 GMT  
		Size: 37.2 MB (37160030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03ededf19de330d97ae5f2cd78f381456f81c19eb46ff80cebace0dbe476eac`  
		Last Modified: Tue, 27 Jul 2021 04:28:02 GMT  
		Size: 4.1 MB (4095072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ec3f753c3934e1f67de00b1cde7c52b2558b372872daab551be31f8ee74787`  
		Last Modified: Tue, 27 Jul 2021 04:28:01 GMT  
		Size: 4.2 MB (4241926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:789a4f765c795159ddccf8f457f9d840a91044809c509cd9c981b46a6a30fc40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34469517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec3ee9aa9f2830da9e12633122859d0a30def2b2379bacc0ab5197a26c69dfd0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:26:43 GMT
ADD file:bb6f157473f0ea3db5bd41bd0a677ea97ea42f69f1e6892bd93a11f1d0df3d74 in / 
# Mon, 26 Jul 2021 23:26:45 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1cb6bfcdfc860a46ea0d0d91c41b5ccb42de505a028d05790a619edb8598f27d`  
		Last Modified: Mon, 26 Jul 2021 23:46:53 GMT  
		Size: 27.2 MB (27183722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf3da92b2a7caf59277ec7bc7dbc5fee6fccb9c477fb7e954947ccbe3c77ed4`  
		Last Modified: Tue, 27 Jul 2021 01:18:48 GMT  
		Size: 3.5 MB (3482612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d1efb8287f1d3a00e174422e0adc42e5fb1db3342f30e40b64d3650851fbbe`  
		Last Modified: Tue, 27 Jul 2021 01:18:47 GMT  
		Size: 3.8 MB (3803183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:42e5d00e6bf75f3cf33f0effc7c57b427c407ac1664ef2b864f8b79df5174484
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40402544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42080f3ab2698fe443a126a7fc56cf1332253256751cd177aa5489dbe1102387`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:42 GMT
ADD file:b6ec59f7691777c81f8a8700ed1da1845eda3e628f2711f38e3c61e05d7a4135 in / 
# Mon, 26 Jul 2021 20:55:43 GMT
CMD ["bash"]
# Sat, 21 Aug 2021 05:09:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 21 Aug 2021 05:09:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:983c674c63ce4a2e843b63eb159ebc7a37998bed4be834de0311107fb837ffba`  
		Last Modified: Mon, 26 Jul 2021 20:57:48 GMT  
		Size: 32.5 MB (32489596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8862aaa40ac181b45b13f941125944e7f6c13aef3acfa0394b2249a8ed5a00`  
		Last Modified: Sat, 21 Aug 2021 05:17:29 GMT  
		Size: 4.0 MB (3950197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdb48f01c6436ddf9b3a8be46c2bb5e7c99ed6a100a8989efff8ed9c4c23233`  
		Last Modified: Sat, 21 Aug 2021 05:17:29 GMT  
		Size: 4.0 MB (3962751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
