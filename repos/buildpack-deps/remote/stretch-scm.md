## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:fe1e0eb9a6e8f0d8c49cf755832f2c595705045a81c3565cb4870007b9f4f20b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bde6538667fbb9db16fd3612ce32f3c578b8e201c4164e46d8eda6cfd65d5769
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110837977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3619c3d8e7d0c268cf6a261fc0df33560b570c662f2a3644425af5f56a786ee4`
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
# Wed, 20 Apr 2022 07:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:2f75d131f4060950dd6cc1f580e2fa5504ece8d692113a9cdb0a866637b397d7`  
		Last Modified: Wed, 20 Apr 2022 07:09:24 GMT  
		Size: 49.8 MB (49765440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:71ffbe15c3b081c0f4ee9ce90707685c3f66a7b3a5bab14d1e6f7824af4edae3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106626237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19832e0ce3b29a5810a63e5841bbb0844498386c7f422132eb495146394ac425`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:55:32 GMT
ADD file:4e79cc43996ddc8062073aea4d6352c3ca3c736e9b09f1eb440f913d5a52469d in / 
# Tue, 29 Mar 2022 00:55:33 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:56:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:56:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:57:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58c023b263eaa1973763831b149ed127bbe67ee8cae67d60e261db1e9d54b63`  
		Last Modified: Tue, 29 Mar 2022 01:12:11 GMT  
		Size: 44.1 MB (44123307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0117421f3f6b9a01b30e38d3562bc7a42dc789c5af5f80877e67cd59edcb5`  
		Last Modified: Tue, 29 Mar 2022 08:14:25 GMT  
		Size: 10.4 MB (10352487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c612024a40834a1cb0833f65b0e86ed44bcd14476cd83a108eca13607211c477`  
		Last Modified: Tue, 29 Mar 2022 08:14:21 GMT  
		Size: 4.2 MB (4162114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85145e2987592dd2778a62d3efaf2f38a56d30e11db945369406880db586d665`  
		Last Modified: Tue, 29 Mar 2022 08:15:12 GMT  
		Size: 48.0 MB (47988329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5d562deef32b025ad53cedd4fe1a890df58eafcce56ddc72d9faedacce8c9139
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102157981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae971d6dcac9b3da6902893bc8fca06305458a725c43d3f7d9ac7a3a785bda2`
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
# Wed, 30 Mar 2022 20:18:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:842f17f357dbe1ebb8ad0508d83e0bcbf9dd99dd8dc3a9084a153a6c61aec7fe`  
		Last Modified: Wed, 30 Mar 2022 21:39:26 GMT  
		Size: 46.1 MB (46128132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7aae2fe6a85e25e4f7672f9e569c6b0a86426f9f6a17b2791e153b9a5a0c31c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105040364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a05a4c878d185f5752394ae01dca1547c510fdc4aef5d91edcf380048cfa0416`
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
# Wed, 20 Apr 2022 06:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:67f90700f5859b0f6187aad3354827bb2b243385f8e4af17fbfd2f81f4867e1c`  
		Last Modified: Wed, 20 Apr 2022 06:57:58 GMT  
		Size: 47.7 MB (47736126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7665fc6bcf69d07c7b7ab2fcfbc22f9338c645cbac8f9cfe9ac95e354b580bba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113116996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709d3801438911257705eaad17d7208ee15626ae062811a930a19c5f70d19098`
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
# Wed, 20 Apr 2022 10:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:3a961561bfa0a5f6fe20a1be17bed015e78fa2cb53a6dfcc0b2b11c2201384fa`  
		Last Modified: Wed, 20 Apr 2022 10:31:21 GMT  
		Size: 51.3 MB (51268708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
