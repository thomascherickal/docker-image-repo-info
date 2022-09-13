## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:20b9d6123daac8f9bbf09ec1033ec6187e2ab3452c25e77ca6a629147071f0ed
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
$ docker pull buildpack-deps@sha256:0cdf8fc2338e2908aae0b8cb9261f56e50595167285a072468eb878f56b54fff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73322397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a98fbb10debdd5ff695d7f1d1c74300723c33abc60ed5431de34067fcb9b2d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:16 GMT
ADD file:7b7161ef988532de9a1ae3caee50f4337a445cd5d88bfe1da455ad45111e2a4f in / 
# Tue, 13 Sep 2022 00:57:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fbb5199f866b772d7999f8d0fead2c513b95972d6d32ec2c8e29311458f0855f`  
		Last Modified: Tue, 13 Sep 2022 01:02:12 GMT  
		Size: 52.6 MB (52643556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5abee259a1d9101a0890f49e244222094315b4c017c58d8cb8a6cc0cd43e833`  
		Last Modified: Tue, 13 Sep 2022 03:52:28 GMT  
		Size: 9.3 MB (9298049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8698192cb686ddacc8322753abf5c95c28d7cca2e06243ec755c2044f89760`  
		Last Modified: Tue, 13 Sep 2022 03:52:27 GMT  
		Size: 11.4 MB (11380792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2efbe808be7ef97c289609e234c974584e97d4992ecfc7d6fb7e99f5508f4cac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71557552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aded14e1beea71efd720acbc686437aefc33a21cc52e01f0a7558316a836b280`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:56 GMT
ADD file:deaaf7142ee9e9a9e95756080e3fc42695c32c1325ff22432d1a8335978dc0c7 in / 
# Tue, 13 Sep 2022 00:53:57 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:27:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2e65672912f1f23209ba2457b7da75b0ac0f01a46e88659ca267298886972343`  
		Last Modified: Tue, 13 Sep 2022 01:01:43 GMT  
		Size: 51.8 MB (51785975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450eec1a6153448c36952598d71f319ac819217fedd3e398f945533effbdd0ae`  
		Last Modified: Tue, 13 Sep 2022 01:33:08 GMT  
		Size: 8.7 MB (8742366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088da11e23af30c629ee1464862f0f4a3fa55ca8c0ebcb8c54f7acd20d8111e3`  
		Last Modified: Tue, 13 Sep 2022 01:33:09 GMT  
		Size: 11.0 MB (11029211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f43c56203997827c84a812462131cbcabc3e4c180f62c92a48595e4fcb79d54d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68633051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b20f50e4edf8c204581294078d6e224f677aad50fc3c310742b2ecb5b6bc19d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:04:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e63ee7b15faa5255a98e78ca57f7b79165de31d27f0d20a810e2e8f2f6fbe`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 8.4 MB (8404984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866f5f3461f124a4ec2d43c116d5e4f8a2783872d85516deec64b8873fb850ab`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 10.6 MB (10590651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7111671eb5e0eef153034060931fed251bc35454d67eaef764d41b8418bd55ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73415245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1f6b44edf551616f54c76b94273bb6cf38ac811641321690130bd55af523ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52438f7d6f6695685610119446105c5c9522703362332bff254bc8eda29485`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 9.1 MB (9135715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c781af42aca050a89e2c2b2ae998b642dd1e62096b74d1479568d49d2b43581`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 11.1 MB (11058895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b9972c98ff602f317e6304009068bc0bcfd55766be4faadef16a50f2e560ac0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75087575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be006906138be6be28f63d53b6777210491d213b2fd95065a1fd6ca582699aad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6de5521fae7f54e276230f1136f3c889618c53b37f387bcb06db2c09c9ea96`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 9.5 MB (9480147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1ad46fde87250408a791d37517179cd6427cd46421e84e138f00437a005cc8`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 11.5 MB (11473735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:569464ecaa8e532d06a96a80c75fc9566c65fcfef99e33ad9bde7ce0c97d67a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72868421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe44fce6a7503ff70aa5e19f32c0daffd778243e3b2135bc88a2819019d5724`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:30 GMT
ADD file:dc60ee74dfccba12269b444dd45f20e0133d724b1942c6b0f9c5194eb68bc303 in / 
# Tue, 13 Sep 2022 01:11:36 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b00b55b6e19db9300c81bc3c7da4bdd60a1432296143ff24c14dc6d0eee819a2`  
		Last Modified: Tue, 13 Sep 2022 01:19:36 GMT  
		Size: 53.1 MB (53078760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86798e592e4c27c8b93559a482630aeb78e21c77d475b6073a710cedc010c221`  
		Last Modified: Tue, 13 Sep 2022 02:09:03 GMT  
		Size: 8.7 MB (8662682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e754dd24f2e4a96086e83f849cac69c8b471a4e9c281073faa059f3ffbe46df0`  
		Last Modified: Tue, 13 Sep 2022 02:09:03 GMT  
		Size: 11.1 MB (11126979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9976e80bc902f0a0e9be54ffe69853a518388672975e91a0dbca9cc51685422b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79287406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a04e630b9a2c28f96e8087ed577aa1796b005fda82c5be6b82cc21d1cfc58d35`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d55c9749119adb9c0cff41513f89896055da109781a9c493c462426691120`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 9.9 MB (9892227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419401365d91198049a8c6620087ce51a751ce8891e8a184d06c31216b0773b8`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 12.1 MB (12081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:4a2fb00746c69ff675e9a4b7c33ca1d49bc7876081e0d523d3d5c0369ce1d8c9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69105062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d5b08235820d175371883da59a21eef0884d079863088dc9f96c4b6e759832`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:44 GMT
ADD file:cf4408ac501f6e39f1a9c7abb24ec07a6bc62afa97f48fd63879c903abfaaf4c in / 
# Tue, 13 Sep 2022 01:11:46 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:57:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:58:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d8cced8b0f3f30b0928735c74d8208eae12a348b798bd4253f1b4acb6d9d6728`  
		Last Modified: Tue, 13 Sep 2022 01:29:57 GMT  
		Size: 49.3 MB (49268300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdf2efe1eb61fd0bbcf2b293d4e031b05f13a19f3ee4f9691262666970b15c1`  
		Last Modified: Tue, 13 Sep 2022 02:42:01 GMT  
		Size: 8.4 MB (8401065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f281e9cb277bf50237e9e04b09169648d24499c56aa01f94bedcadcb173d0a3`  
		Last Modified: Tue, 13 Sep 2022 02:42:02 GMT  
		Size: 11.4 MB (11435697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:31ea8864ee36fe749530f5fa2d599d61820e8d38ce13dc1bf7121f74b4f5fe02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71711809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0a8d1b3e3f918c33cd486c119b5c2746c20d4da7e5c6a3366af0ecb178aa714`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:19 GMT
ADD file:c95e2b098d871c8f60e72d16096a4bcce80e256166b62df3ac0abf8c1cc5384d in / 
# Tue, 13 Sep 2022 00:48:22 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:27:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:27:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a47738c5650c377467230bf819bb4be695718c6effbf5489b6e0fc8e11229d95`  
		Last Modified: Tue, 13 Sep 2022 00:52:55 GMT  
		Size: 51.5 MB (51537006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92aa5a30de3637ebbcd271e1f1795c92f2432d80f355e866dbb37a7875ba82d9`  
		Last Modified: Tue, 13 Sep 2022 01:33:40 GMT  
		Size: 8.9 MB (8935914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2c639682b677cbe7eebdb0376ad10594f99f1d23baa05fe3c38f108872567c`  
		Last Modified: Tue, 13 Sep 2022 01:33:40 GMT  
		Size: 11.2 MB (11238889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
