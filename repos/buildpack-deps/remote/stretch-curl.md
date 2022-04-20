## `buildpack-deps:stretch-curl`

```console
$ docker pull buildpack-deps@sha256:29b6da5f843c0cf80de54426a23710f2c6497f46aedb93af6c2d9ae47f2fc687
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c69b9970f99ba22ff5b702455bfc729c7c697412775d97a1edd1ae8ca5434939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61072537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239d6cd201016f06530d3a6c6e1f93b85fe86be34ef9cd193e36f7158231b34f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:14 GMT
ADD file:6ed691b65385dede44a92f9de9e1428af431197c66461aa0f9c61e2f7c8bade5 in / 
# Wed, 20 Apr 2022 04:45:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:01:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:01:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f5196cdf25181bc7e4411865a2e002932b7b6b0ffce787c04c1bdeaf1f204f20`  
		Last Modified: Wed, 20 Apr 2022 04:52:01 GMT  
		Size: 45.4 MB (45427434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed1e86f01ee95c76d2c8b4385a47ae336e6d293afade9368469d99daa9369f`  
		Last Modified: Wed, 20 Apr 2022 07:09:06 GMT  
		Size: 11.3 MB (11302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e4bdb3a6c1325cc4d40e585ed7a759127c0c87b0388ec0236b1698827d70d`  
		Last Modified: Wed, 20 Apr 2022 07:09:05 GMT  
		Size: 4.3 MB (4342835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:272729c969441134054c43162620fe00b86191ffd27ed2187cd761e1f78c02dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58637082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20afa6d65ac8208485108d5ebc93189186b76dc05f556b636a10e8ca13cfe067`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:22:06 GMT
ADD file:407e28120c3ae0a1012433a9787cf812e0ecc360e63ace9fe21f6728470b4db1 in / 
# Wed, 20 Apr 2022 07:22:07 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:51:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c6849d3c2fa1fe7c2c78db1c26ca92e44c119dd3e92d93450115c927ecb6dce6`  
		Last Modified: Wed, 20 Apr 2022 07:39:41 GMT  
		Size: 44.1 MB (44122673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609e00e6d304c762e4073f3690670af8db0ea1c4f668f7a6f9caabf74e25f`  
		Last Modified: Wed, 20 Apr 2022 13:10:42 GMT  
		Size: 10.4 MB (10352382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ca0466eae214f72298cc4d595c064ace398289b59d9a2c8d89bd50c8f6be4`  
		Last Modified: Wed, 20 Apr 2022 13:10:38 GMT  
		Size: 4.2 MB (4162027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cd68d7d326ad0a0a85ddd2a318d47104d0ead3f07d862634d3683acbd0900753
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56029849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77070c474e93c166cc5ea851be4c59032d1773b9d1b310d0fafe099304e18811`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:23:57 GMT
ADD file:3dc1697adfcf63a288e9ec7a2c40438b8ba2ccfff0382a1ed5457f30d7a37f76 in / 
# Tue, 29 Mar 2022 02:23:57 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:17:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:17:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:aecfa9e0b0179abf68bebbcfc35453928546e01ad1c8b6eaadf759360762dada`  
		Last Modified: Tue, 29 Mar 2022 02:40:33 GMT  
		Size: 42.2 MB (42151158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc36fcf6b269b843685f3e40183609c9ee393c766145d636666727cc97069e`  
		Last Modified: Wed, 30 Mar 2022 21:38:43 GMT  
		Size: 10.0 MB (9956889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e13cc08b3e8cd7b26260c7597b624d4a45ebc2afb89bb5da193fc824ab69e55`  
		Last Modified: Wed, 30 Mar 2022 21:38:39 GMT  
		Size: 3.9 MB (3921802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2f1afd56869357f456428fa234e21cc026d8a91f371d9901eab0b7c9dd1ed656
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57304238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d3ba884d80b06852a27b811a3e102670146cc32a31b9263f91d32e0bb351ba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:19 GMT
ADD file:73f1db8536438ca891f4b507a569e6c561364db0f05914ebea9d3fa97e1bf837 in / 
# Wed, 20 Apr 2022 04:31:20 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:48:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:48:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a41fbedfa4b1547a2b4fea33de48af745d66a94741d3cf344cb2766f0e80211b`  
		Last Modified: Wed, 20 Apr 2022 04:39:38 GMT  
		Size: 43.2 MB (43212018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94d3b1a91a1952461644c0005791faf07bf7c6b042272a89113ec795a493d4`  
		Last Modified: Wed, 20 Apr 2022 06:57:40 GMT  
		Size: 10.2 MB (10217775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad88c3c2eedd19cb4e591bedf0013f98bd12344b922299e40887a253d50de12`  
		Last Modified: Wed, 20 Apr 2022 06:57:39 GMT  
		Size: 3.9 MB (3874445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:349e2149f58dc4eb45d0445d88b9d8837a93e1820feca78af6e8bf262d4a9aeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.8 MB (61848288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0261aa0b2cb1e5d1584f9ef2f63298ef01a7ebf9af00ec5cb840b806031167`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:57 GMT
ADD file:e8c6a60834ed931ccc3c93b1f2c9b9ca2bf190b0d8d2474382ee8e96a7e35b5a in / 
# Wed, 20 Apr 2022 07:39:57 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:22:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cd343d4c0c2fbc67ddea33155621bdf36074fc30ffb6f917e716fbb81645f79a`  
		Last Modified: Wed, 20 Apr 2022 07:48:48 GMT  
		Size: 46.1 MB (46147730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b0c0f848ce870a8686c5b8c6c955359aa284d4e35847ab4c25247e6ad8c855`  
		Last Modified: Wed, 20 Apr 2022 10:31:02 GMT  
		Size: 11.4 MB (11358258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ca979e8a7a5453cdea6aeecd54c837a03c2c5c037a42ef4cb105a69783071`  
		Last Modified: Wed, 20 Apr 2022 10:31:02 GMT  
		Size: 4.3 MB (4342300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
