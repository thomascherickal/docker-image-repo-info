## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:13c8b3a9a0a47e25fcd96c2c2f25f40a80e7ccfbde695f7b4812663e763e9c06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:876cfe58c039fd813ff318d4e53e2707c884cb7b8c7952464dcf2e27cca17b5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71783901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:506d6fd65061be41934c131b48e3c840c7e841b27244c6d3c657f0c4008db311`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:53:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b8f6b86e3a84210feef982a4953fcc1b15003e51b2fb7b861ae18f18e914f`  
		Last Modified: Tue, 28 Sep 2021 02:00:14 GMT  
		Size: 5.2 MB (5181002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e6a19825e33b3ebf505b0ae79fe6cf49091e693c4d8971abde683746f445`  
		Last Modified: Tue, 28 Sep 2021 02:00:15 GMT  
		Size: 10.9 MB (10900815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b9f458071c07c1922362c241070e5e92fcae56e600b5fba756c6c7f016a7b8dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68653424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e3b381e72d26f967883d0038a368254c7a7d6c8a34171e0360b55d6a190f08`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:53:41 GMT
ADD file:9d67c83a2e727f33502861325786047b9c6034b490854b93efb2d59cf973e5b6 in / 
# Fri, 03 Sep 2021 00:53:42 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:39:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c25501d6a46457c5895808abc531a7dcd2b4008bc42a432fcd73b6325c3fdacf`  
		Last Modified: Fri, 03 Sep 2021 01:10:41 GMT  
		Size: 53.0 MB (52980070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ca497a6979f627d04639faa5571c98e112e1c56465986fce9d78c17101a5ce`  
		Last Modified: Fri, 03 Sep 2021 02:57:25 GMT  
		Size: 5.1 MB (5077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eab0927e6f1d00c87c3eed02237eb8b36a819bc0188dabfab4074f096423576`  
		Last Modified: Fri, 03 Sep 2021 02:57:28 GMT  
		Size: 10.6 MB (10595736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:be78849522bdcc5ff98e6d4d7a8eab865c7d51db902caeeed25a179e8a377c2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.8 MB (65814390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486fb87003d8a41efa70353de3d661a1c88f2673444208de043f980549fad132`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:03:00 GMT
ADD file:78431ef521d2864441ad8fd6f5238d8c49ff519c7f8510394048cc042f270288 in / 
# Fri, 03 Sep 2021 01:03:01 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:59:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:59:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:669a70f2eaf280942d3e643fd270beb3d6f313daba0d40fa8f3a72810a1e9bbb`  
		Last Modified: Fri, 03 Sep 2021 01:19:37 GMT  
		Size: 50.6 MB (50637968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df9116db71fd664add238def53f5a22bec8a3292c6838466fb4f27cab0a4f32`  
		Last Modified: Fri, 03 Sep 2021 03:19:09 GMT  
		Size: 4.9 MB (4938329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370eb59a5763f3c415a9a5237b8e0f6513d04e87645086ddebd2c455a1322e1`  
		Last Modified: Fri, 03 Sep 2021 03:19:10 GMT  
		Size: 10.2 MB (10238093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:05471b2a55694de5fdfe1140b6455177d9be98ba20e75ed6bc90ab299f93b57c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70580947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8a219a5f678992a06e3dd89d706936f38b3999a8ad111dd393c37e2f4127f0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:54 GMT
ADD file:e9cb8fff7ac62f9bc8a4ccbc3960693736104975b5c3ffc855a1b6dea13b4c10 in / 
# Fri, 03 Sep 2021 00:41:54 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:35:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:35:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2cf0882b72727438ab6f57aa6a77711053bee00d53c08f527d6fc8e582fcdb3f`  
		Last Modified: Fri, 03 Sep 2021 00:51:39 GMT  
		Size: 54.5 MB (54529119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5fa429768d201e6729375041d9f10e3f1c4f37f2be592556628bd633b52b63`  
		Last Modified: Fri, 03 Sep 2021 04:43:31 GMT  
		Size: 5.2 MB (5160231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e36c7a8c3d951e4bab7bb201143c723a1db2d463482ff21f205c9a80f4d132c`  
		Last Modified: Fri, 03 Sep 2021 04:43:31 GMT  
		Size: 10.9 MB (10891597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:172f86014cfd23f8534f1d81a96c73a480f0fcf8f38814951938b8646bc3cf67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73100008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ceb13982ea1259ee29ad6b3ac68115fee570615ace45461936af7d9edd4e5f8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:41:36 GMT
ADD file:64515d15f0b2fac0544e320a88716de6bf306c10f7e9400a945fca420a730843 in / 
# Fri, 03 Sep 2021 00:41:37 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:965ebee0ec76f6f76a0d14e40b7923292e9028532546ec1a748a8fed8267c897`  
		Last Modified: Fri, 03 Sep 2021 00:51:22 GMT  
		Size: 56.5 MB (56525268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56089068afb291eba965e50fb15a03f5ae7c433295ed8d952822fe54d1c1dd97`  
		Last Modified: Fri, 03 Sep 2021 01:22:57 GMT  
		Size: 5.3 MB (5303864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab52954bb9b6200d56553ce69fb7dae734a92c479ff8e38af69fa29a7d28110c`  
		Last Modified: Fri, 03 Sep 2021 01:22:58 GMT  
		Size: 11.3 MB (11270876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0742b4ef0a1e6d36f6a1baf7431d7ce25444bf9575509f0ba031b8b243cf1251
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70167872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fac613c7b4b40ce813d10d55b6b0ad58587ca17e308844e5aa980796ab1392f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:12:04 GMT
ADD file:d3a974d875f356507b0ce365ec750c6109f909b93c690b9778a4c115aa14a20b in / 
# Fri, 03 Sep 2021 01:12:05 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:53:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3d38c5abd667c8252a6e859616365d153c0ebf15516c401ad631183f19343ec1`  
		Last Modified: Fri, 03 Sep 2021 01:21:53 GMT  
		Size: 54.1 MB (54135005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8b578c68c33ad5ddf748ce7497de380f1903d441aee0c8b0b1af0471180e1`  
		Last Modified: Fri, 03 Sep 2021 02:04:43 GMT  
		Size: 5.1 MB (5132409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a57f2a02c7810a593cba16221fab32426c75881bc128a91ef728048538e53`  
		Last Modified: Fri, 03 Sep 2021 02:04:45 GMT  
		Size: 10.9 MB (10900458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f686e9380a7ddf6bd2900de9f550ad307efaec5625ed23c223f0bc49e5b4eb11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76607648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:458f349d2522ffbef1b1dc6a5f6f49b9c4cec344f768cabcf7a36baec2536acd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:46:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a95302a54a7fa51cdd0cd0117968b05d9f71d3c40eafe66873816a3b43ba14`  
		Last Modified: Fri, 03 Sep 2021 07:14:06 GMT  
		Size: 5.4 MB (5422617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da11fea16e40da1a9b66dee60a49dee27fffb468c778b12670ed59f3cd11837`  
		Last Modified: Fri, 03 Sep 2021 07:14:07 GMT  
		Size: 11.7 MB (11650959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:bedca7b6c6375e09dd1ffb3eec3b607a8b8b9a15dd142b77525579bde87a41b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66588742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183f6c97e7e26c4086f4b6cb32c3908d6b090e56eab64119950c4a699dca29b0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:16:10 GMT
ADD file:22169a464bc792387d0c6cd4ca985b70527601306f274a47f7a26223b125d1b8 in / 
# Fri, 03 Sep 2021 01:16:13 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:59:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d209f64ed888c716b8fc1f768d766ccf831d8a034eb5e3ca12945873acb106f6`  
		Last Modified: Fri, 03 Sep 2021 01:32:35 GMT  
		Size: 51.3 MB (51289049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da873824fc3fcd77f59d7598fa94a4e0eef799c270584961cd61b0193ad259c`  
		Last Modified: Fri, 03 Sep 2021 02:39:12 GMT  
		Size: 5.0 MB (4986349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfba85c856d5ce39bea54898a8e2d95aa9c37df4c646386dfd0d1099c262561`  
		Last Modified: Fri, 03 Sep 2021 02:39:16 GMT  
		Size: 10.3 MB (10313344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b734c11fedc4319a44595c49e3541d7a69e4c3bde2e5b12f1082ed915b59a556
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69912708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f80b8e561ff61c6a6d9bd4db8e89f29950f901bce96b85d1b662f440d23f5c4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32362b87984c1bba14b0f80546944827886c7cc7accd0865b4ccc7f34a9f3b8a`  
		Last Modified: Tue, 28 Sep 2021 02:17:31 GMT  
		Size: 5.2 MB (5165065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aadefacf33492b3a74622a982ea04f1605a554feeaa2ef0abdd214a94280744`  
		Last Modified: Tue, 28 Sep 2021 02:17:32 GMT  
		Size: 10.8 MB (10793806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
