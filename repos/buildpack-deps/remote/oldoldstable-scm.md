## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:ad233aea2706b096e637b613e4dc0a74ffef86b0b0e0b987bebdad254812b30a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

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

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

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

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

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

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

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

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3953fde6341827b65993d0458257cfec1c0f998bf470b62645672927eeb34964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113115686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ac52af2aeb2680cb19b9eb2d663dc5a9b067328a5a4424a96cdafdf3a01766`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:44:09 GMT
ADD file:74aa6d4005ba30e0fb6af0b75158bccd03c55e837be6f73f1c2929f62028a19d in / 
# Tue, 29 Mar 2022 00:44:10 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:02:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 18:02:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8b8952dbc41a74d8004d044b352e7f612041bf00ab66401180cd3af79d35a14`  
		Last Modified: Tue, 29 Mar 2022 00:53:10 GMT  
		Size: 46.1 MB (46147573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434a4f3f3baec793c431715991d82fb56bfbd9cf0a0bbf4279af77c453529ee8`  
		Last Modified: Tue, 29 Mar 2022 18:18:40 GMT  
		Size: 11.4 MB (11358228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f9948fe9b0550578499ca71c9ec007e18340e37504109404d1b54634960324`  
		Last Modified: Tue, 29 Mar 2022 18:18:39 GMT  
		Size: 4.3 MB (4342256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fe7fe28ce5da9cf227db9f102ead8076b04ec82e230f682c42a1fdfc441795`  
		Last Modified: Tue, 29 Mar 2022 18:18:59 GMT  
		Size: 51.3 MB (51267629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
