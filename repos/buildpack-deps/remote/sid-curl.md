## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:fe80167ca673977d82215a5a47b979c0d02e4b6c4d833be3f6e56cfc4042f71d
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6f236c8191a9698c9ae04e4c0058f22537f55f4e2cde67e1ef9bc7b0a3ca8b83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73809467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bcbbb457890e1d373f7954b7353e609e2600449c290f6ff351c10273d577d0b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:52 GMT
ADD file:8f3d1b2e7474fdc04cd1135312dce29db677e5567ff094e59c8338f5bd2465c5 in / 
# Tue, 02 Aug 2022 01:20:52 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:49:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:180517453f08358cf15a4972d7eafc4c2c649be2333940572c68856727b63bdc`  
		Last Modified: Tue, 02 Aug 2022 01:25:57 GMT  
		Size: 53.2 MB (53231560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea3bb192fc1a2203afc9f801c7c8a19b9753282603b3c8a634578bb887beef`  
		Last Modified: Tue, 02 Aug 2022 02:20:42 GMT  
		Size: 9.3 MB (9305398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd36f037efbbab2cd1fcf04b9f87ba901b2835ba77678dbf9521f200b225fadf`  
		Last Modified: Tue, 02 Aug 2022 02:20:42 GMT  
		Size: 11.3 MB (11272509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:71e2c01c10738a2393e1de893af0ba2af96f670e69ba1247ff4b341d90328bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71709647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40fb8851f698beb9ffdb247f1c155484eab3e8768974b75caf70e82830d33b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:50:23 GMT
ADD file:2829a8dbc1e67454e67c0015efaaceadaa4b04330ed9e60cc8248246cac2aae2 in / 
# Tue, 02 Aug 2022 00:50:23 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:25:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:25:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11a67d4cf31e6e9dc8797a5c01d3198f326d91410c372d1a490bf5592578d9b1`  
		Last Modified: Tue, 02 Aug 2022 00:58:37 GMT  
		Size: 52.0 MB (52021372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6833771528bea1307d56591db306804d9768947a466a60b5de4f6b545ab0cec5`  
		Last Modified: Tue, 02 Aug 2022 01:33:35 GMT  
		Size: 8.7 MB (8741294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2288f8703c485a4ea82b9d9a1de8905ae4f0e420ca4f317625f441977a31c0`  
		Last Modified: Tue, 02 Aug 2022 01:33:34 GMT  
		Size: 10.9 MB (10946981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6a1dc7cb1cfabd89e6d480fd7636b4982c9b8d7938703b686a3f106e6730956a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68748018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:836d2baee2173e1ced99b95dbe1a7c3bfc11ee36f69245661672947313a3bcc2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:00:45 GMT
ADD file:a1d27fd37cd41b3026c10df50adfd5a93a40194548a87a372c97149f63b096b3 in / 
# Tue, 02 Aug 2022 01:00:46 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:50:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:23e34b183a37464e321571d2a75fa33fded0e5a8506066db5c4f20153a665c2c`  
		Last Modified: Tue, 02 Aug 2022 01:09:03 GMT  
		Size: 49.7 MB (49735351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af50b5c584586bbf2589138734167dd8e14560e75cd854cd9bca75019a3f530b`  
		Last Modified: Tue, 02 Aug 2022 02:12:03 GMT  
		Size: 8.4 MB (8423017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4818fead9ad7b4ed572aa86d08f341272cc2cbb418cbe22f7f7d71f2be3778d`  
		Last Modified: Tue, 02 Aug 2022 02:12:03 GMT  
		Size: 10.6 MB (10589650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:862e19141101ececdd8c8b4b921d9c66454cb29054c94150f924f060b9e1b670
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73524133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65fb6c857675349da2e7836394fde759284d1652aa07a8511357c92c56779c68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:477966410dd9e274b01740d7af857db5c024b4c4e53a5e83b5da6854d5b0c209 in / 
# Tue, 02 Aug 2022 00:41:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:27:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:27:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17bcb8e39c7f35480d4c2e5b46b6c0a58dac180206453cc49052707aa8053632`  
		Last Modified: Tue, 02 Aug 2022 00:48:00 GMT  
		Size: 53.3 MB (53311787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e49dab65b12b89c427063ea6eec0802e14801664648c428e5a774754f3e73`  
		Last Modified: Tue, 02 Aug 2022 01:47:00 GMT  
		Size: 9.2 MB (9150009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b71a9f562c782f5916aedb7846293c7057b9f5f32ac072f785d2b21839f530`  
		Last Modified: Tue, 02 Aug 2022 01:46:57 GMT  
		Size: 11.1 MB (11062337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c67559d97bf8d24c807b7d0264b3b96b025e99b68e3da26eff1bcf87d7422bcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75148829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68262f81d60c0f5be2b177bdec794c3f92b300c62e1ce7d1dc80d43a7e6d5109`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:23 GMT
ADD file:40a2042e14b22d803da216af628cd6e8603c923c4fe79ca3c4c79c95c1c1e878 in / 
# Tue, 02 Aug 2022 00:40:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:12:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:12:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ef86b631f45587b4b6d1c16b80732997a4895ae8df072b14d68c25aeff8b901e`  
		Last Modified: Tue, 02 Aug 2022 00:47:20 GMT  
		Size: 54.2 MB (54195066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4385d16696693ee42b7a7f20009fa801f71ca0c6e014ce30f294f40d9993e965`  
		Last Modified: Tue, 02 Aug 2022 01:26:51 GMT  
		Size: 9.5 MB (9480230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed00b31a2aacbca3fdd1dfb26c6e14bf0bfbd4ab13f2498063fe7786ad715669`  
		Last Modified: Tue, 02 Aug 2022 01:26:50 GMT  
		Size: 11.5 MB (11473533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a066927b5ec09a3c745cdb27319b860af8d276f3d23efc2b091f4a9a10370066
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73007477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b88a966c0901785dc7b8096d2394d610676b405eebe695aac588ab352de1cb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:13:16 GMT
ADD file:6165703835b4dbffafda027e272e21bf37cfc276085814fa1d03c1db0162e605 in / 
# Tue, 02 Aug 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:11:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:71112f7b4dfd928d54aaa23ee1023fef50d2dc747bf6e2168afe69932ce8aa1a`  
		Last Modified: Tue, 02 Aug 2022 01:24:23 GMT  
		Size: 53.3 MB (53305987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523353756f561bdc5914e25ea1cfeda5bc330e894285664b88d8ce11aa594a29`  
		Last Modified: Tue, 02 Aug 2022 02:30:34 GMT  
		Size: 8.7 MB (8659688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2258650534e83b3efae8fb3f1ce269322b09b63e553775a7c0b8c8104b2451b0`  
		Last Modified: Tue, 02 Aug 2022 02:30:34 GMT  
		Size: 11.0 MB (11041802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:06cdfa0e53f775de781a7ca8df696f077aa8d11900079078ba6d09ffa6afe1f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79414372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aff993c0b06ebb20e22928ce3857f84fb8df00f14907bb609468fca58d3182c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:52 GMT
ADD file:6911368d0ae9ca029c373628ddb642f29cabf3f909e9a77f8931355843b8ea49 in / 
# Tue, 02 Aug 2022 01:18:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:35:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4a386a4ce4974e6c6fc3a96c6a7a96ce47fa8df11122fa0a4b856c23c5ccb46b`  
		Last Modified: Tue, 02 Aug 2022 01:27:09 GMT  
		Size: 57.4 MB (57440227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eae2292d82f6824061d200408b3f0dfb525d1d5fcf719a2e4c01a7c4c82aea`  
		Last Modified: Tue, 02 Aug 2022 03:17:23 GMT  
		Size: 9.9 MB (9890501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465fd13cc41c21f92aad774503ecba5a1a350a8ee1c0affd0e437746ba26a774`  
		Last Modified: Tue, 02 Aug 2022 03:17:23 GMT  
		Size: 12.1 MB (12083644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:97d8953f17a0497e3fcf78bdc8fc7d9ff057a47664ce8389ea65a6f7c1108ee6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68493959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9706e4374b4ccc49644ae5876124e0e5e0898041f24636de5fad5fff80ea42`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:38:07 GMT
ADD file:ccd99a55cba9f7182ec3cee92173a09fcce1434af80adaa233b43e053b04cca1 in / 
# Tue, 02 Aug 2022 01:38:09 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:09:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:10:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a436e5274dc38943f852c6102f483221b16db3fbdcf3cef362be756d16ce7b39`  
		Last Modified: Tue, 02 Aug 2022 01:56:31 GMT  
		Size: 49.4 MB (49420055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a5bfac3eb41db01442d876bb3d5a4e9eb6a032b82029bae382e090696e61a`  
		Last Modified: Tue, 02 Aug 2022 03:14:33 GMT  
		Size: 8.4 MB (8415462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad6a51628ec48f2096a03efceeb8af7e0189526c75e69b3189928b55c3b25bf`  
		Last Modified: Tue, 02 Aug 2022 03:14:33 GMT  
		Size: 10.7 MB (10658442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e7c48a4d90ad2c746b43f0827ca881fc92ec57c70337fd9e24e589de09a2c2c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71862403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5bfaae2997e205011a76eae3acb25d30ce8a2d7ee833c538bd2355a4dfcca40`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:43:36 GMT
ADD file:19dee33de85aac92620de3bd92768833a889db0b60b7445419bccb4285c46f94 in / 
# Tue, 02 Aug 2022 00:43:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:12:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:31888e988211ae2cd4058438d0fd3d3420a26d35f21e97741527c1e85ad2d476`  
		Last Modified: Tue, 02 Aug 2022 00:49:29 GMT  
		Size: 51.7 MB (51734666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd60a4351ebe5fad9f32c09d0a6f7ec29b6c6dcb5ff8c29e6650149557447e2`  
		Last Modified: Tue, 02 Aug 2022 01:36:55 GMT  
		Size: 9.0 MB (8960873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440b0db795ce4385e2a159326c7d9ab52e109942607b82b1c377894e874e601d`  
		Last Modified: Tue, 02 Aug 2022 01:36:55 GMT  
		Size: 11.2 MB (11166864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
