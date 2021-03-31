## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:c27e6ac0e4670d20844e8350f7a7ba82825dbf3d0253659045e10974aeaf4dc0
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:974dd076d6ecd16d4c3c931127aff7dedfafc1971d4be553f29ac8006a6c2267
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70886655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1dec83dd8ccd9f47a2deaec85d1c922ca62c7e4ddc8917304fc691a4ece4f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:48:53 GMT
ADD file:32519b03930d9f5db9010ae49e0987322ce19eab681ad5c841fe1cd6268ad2ee in / 
# Tue, 30 Mar 2021 21:48:53 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:00:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6abc78d8e2422868f293b265b6c0ec3ba250fc4987f862ba05e86d7eb277f297`  
		Last Modified: Tue, 30 Mar 2021 21:52:53 GMT  
		Size: 54.9 MB (54868089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1424cff1d2b47e24acbeb3381319a9bbefd1f8dcae5c521f0198833d9b2911ec`  
		Last Modified: Tue, 30 Mar 2021 23:12:47 GMT  
		Size: 5.2 MB (5151423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859f37c645b9a1a4967007d3e310ace7f83d9924b7fd77385ff9e2de20a55a5a`  
		Last Modified: Tue, 30 Mar 2021 23:12:48 GMT  
		Size: 10.9 MB (10867143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:708640ea74b199eefc7fc2044533bf72ae62ccff77512823055452c4a7cf3efb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68032145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cf7e4f2e53484e673e6ed43d79c062c646797dbafca540285c04829be4c332d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:55 GMT
ADD file:3a982d4cdc7d9461623d85a4b6162531ca9adf2921f0d43a0b548d3710392387 in / 
# Tue, 30 Mar 2021 21:49:57 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:43:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:43:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:645891123da6b320ad4fd8cfadf96c77b7144dd25b617222de1fe718cde77e35`  
		Last Modified: Tue, 30 Mar 2021 21:57:27 GMT  
		Size: 52.4 MB (52401170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e2ae11e65cec397d581f8bfc50a0c3eb2d363cc2397beaa585ac385f720fcf`  
		Last Modified: Tue, 30 Mar 2021 23:59:40 GMT  
		Size: 5.1 MB (5061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131fae12c09181b2c23186780b133bfe60e76c8af6bc6af4943aed293c993b47`  
		Last Modified: Tue, 30 Mar 2021 23:59:40 GMT  
		Size: 10.6 MB (10569881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b32eefcfcf8c2ab9a9f795d13c1df92c7d83db7e5f11e96e72157990f2a5cdb4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65212234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a228ac2c3d7ab2ad2ca9cae3cffc504a7738dbf4505065d7121beabc5fa51ef`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:15:27 GMT
ADD file:e3651409d9338da981cd9fbd8d9b8511edbde0700ac9e0df8937b859e004990d in / 
# Fri, 26 Mar 2021 11:15:29 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:16:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:16:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dd9021b04def024e25507cdd1b0967a20a384ad5cc255120cfb8c5f43495fa74`  
		Last Modified: Fri, 26 Mar 2021 11:26:11 GMT  
		Size: 50.1 MB (50073977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6023b28762fcb2cca84dd988c0545da69e2cb9cea40e5fb1a14dce3d7d186`  
		Last Modified: Fri, 26 Mar 2021 13:48:58 GMT  
		Size: 4.9 MB (4920097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94408c405dc2689a60515a2dee289cb3495f53f4b4f9758de6995e07aa073eb2`  
		Last Modified: Fri, 26 Mar 2021 13:48:59 GMT  
		Size: 10.2 MB (10218160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b02c69efbfa57df7377e99618645facf16d8d50cdd683887379754a6ae8cec73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69563410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cfbd0da1959b711431b6b8cda5072c765df4180ff9df4d0db6121afe214573`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:09 GMT
ADD file:d2b87aea7c45e4b0e478e3c2eabae00f1c80b5d77f8f579d2ff913c78b44b6b0 in / 
# Tue, 30 Mar 2021 21:46:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:11:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1063bcb9135253bd841aad1946f348a3277d992a7ecba4ef1ef68217c3c1b019`  
		Last Modified: Tue, 30 Mar 2021 21:53:23 GMT  
		Size: 53.6 MB (53555197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890e5446d487fcab6d7189e7771c6a50252b2d857c9b70fd4cea1bcfe3a1c8a5`  
		Last Modified: Wed, 31 Mar 2021 00:28:24 GMT  
		Size: 5.1 MB (5140737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b996f43aeb591ca2dd4bc003c5c5e3e982c6b85b7cad5a14591b08209f01b95`  
		Last Modified: Wed, 31 Mar 2021 00:28:26 GMT  
		Size: 10.9 MB (10867476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0633531ade49076142ebfa87b645a4ff3be5f5abfa2fc7f9bf40a95d506a99ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72410188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f628e9661cd0bc768dfa25de1aef846b9f69f8fe6a5122848c058ef342c077d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:38:58 GMT
ADD file:b5024008ca4ac295c015d04d146515efd534f38efa8793979ad8a6c1cc41a2b8 in / 
# Tue, 30 Mar 2021 21:38:59 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:54:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:54:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:46dc83097f0241a9cf1128d563661cf2cacf0ca9445152008a4c686a8d125595`  
		Last Modified: Tue, 30 Mar 2021 21:45:11 GMT  
		Size: 55.9 MB (55881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96203cf1270a0522cb74805c17be141b6be163c96591b032d0aeceff808d7b6f`  
		Last Modified: Wed, 31 Mar 2021 00:06:09 GMT  
		Size: 5.3 MB (5280209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63af79a424e53c82e0807d0e90f60c2456bc0ce3accdcee7cb3f1f9f5f70a96c`  
		Last Modified: Wed, 31 Mar 2021 00:06:10 GMT  
		Size: 11.2 MB (11248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4aa4fb739863fe7d29e922f8cf48cdef98817ea28942037efed908a72a6c39f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69110390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822c955f59e593aed137ee704e74e27c786999f8ce16398c74895725ced3748e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:08:38 GMT
ADD file:4c1773eeb1eb8715f5ee35943b6ec536fef99670907da849b45a0a757fbba521 in / 
# Tue, 30 Mar 2021 22:08:39 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:06:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:06:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a1bfb759abe39ebb60de9072afdd4e8e520a2faad8d254176313a6e6015b23b2`  
		Last Modified: Tue, 30 Mar 2021 22:14:13 GMT  
		Size: 53.1 MB (53127187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9534d5829810d03b9be336ae682a19f3b3af31e49b6b2cecd48345d02bd56074`  
		Last Modified: Tue, 30 Mar 2021 23:18:40 GMT  
		Size: 5.1 MB (5112994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efe461f21748a446fa26cb598f3c639bb1d56f946ec69917e33bbf0d1afe79b`  
		Last Modified: Tue, 30 Mar 2021 23:18:41 GMT  
		Size: 10.9 MB (10870209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3c0cd9061b483b0ee7e38574a3070efed8495b58ff91f1de84caf983232d5518
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75775545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427fcd31ca49cb171d7712aa16e7e2eb2ddbe26aeb2e034f19fa3658bd1a7fe6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:12:40 GMT
ADD file:28f7d129aaacc2de6bb78dec104b788d0aa25aaac87e07873668354a5b755268 in / 
# Fri, 26 Mar 2021 15:12:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:13:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:18ddfb418fe2dc2d92f9b851d0345827010c7b001ef98bb5a8b1730d80e2eace`  
		Last Modified: Fri, 26 Mar 2021 15:20:35 GMT  
		Size: 58.8 MB (58756702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e58f4581a73db06180cd5d10d619dc8b47cdbf57bed71dbf9eb53d28bc4749`  
		Last Modified: Fri, 26 Mar 2021 19:34:46 GMT  
		Size: 5.4 MB (5399177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e302f47f5e7c563d0f23745e32bd160587a44a206808295a2ca9d29a6b9d67`  
		Last Modified: Fri, 26 Mar 2021 19:34:51 GMT  
		Size: 11.6 MB (11619666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3f10991bd84fcc950adbf8b9c3a98533f8479716a071ace54e0f33769acd13d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69040934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff333dd7658e28574df55d411c882c8010f695313682fe0df279576530ac3c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:00 GMT
ADD file:06cd9dd574d91229d3aa7c645dda03791fcfbea17bb5964aaa1c5830d4174ab2 in / 
# Tue, 30 Mar 2021 21:42:06 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:41:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1babe08b94dd6b44aca97f5f46b49d3c3e8b1571a49971cc87c69f9c91056218`  
		Last Modified: Tue, 30 Mar 2021 21:45:29 GMT  
		Size: 53.1 MB (53148454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870ee6737fff361d9c0e6f905afcc7d45e779397ee67aa5b284eea46c9bd446d`  
		Last Modified: Tue, 30 Mar 2021 22:48:10 GMT  
		Size: 5.1 MB (5134079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54e0f71a88fa90537f4f2b0b092586cde9dc64e5833c45246c5d15be4e2ea20`  
		Last Modified: Tue, 30 Mar 2021 22:48:16 GMT  
		Size: 10.8 MB (10758401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
