## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:90198adb43d5312adcd5515e9f70938375f6aa793ba0cc0646e0f205de888a6a
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:55dd6d36335ccfc0da3d5a85468a4e1f483a90b05a195b9ffcd8262e050c512a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128797024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f680313dc1aa142af965479afee8830bafe75bd5306104e1b552b7e8f5ceebd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:58 GMT
ADD file:69369feb027cb9fcd22f8a4b51431458f4e51eca8bb0c398edde4cc47c3d74e0 in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:15:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:48c02bc8c594d3500557aad8d76d43fb3cd9632de373f64648f0523fd33f3197`  
		Last Modified: Wed, 26 Jan 2022 01:49:14 GMT  
		Size: 55.8 MB (55811672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05b5335d4dea27f0ba29bd1ce5c5b9d3b0ab8f87964be3312ecadc0f34e96`  
		Last Modified: Wed, 26 Jan 2022 02:24:56 GMT  
		Size: 5.3 MB (5274876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dacb71892995084387b6a8a0a9ac7eae9ee1b597031f8e25ee46a18d91140f6`  
		Last Modified: Wed, 26 Jan 2022 02:24:56 GMT  
		Size: 10.9 MB (10915453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b478847de2f32699c8d076c0b8e04755dfe8ff874f85e216f02d790059369ec`  
		Last Modified: Wed, 26 Jan 2022 02:25:17 GMT  
		Size: 56.8 MB (56795023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:08fb4278d267dae61ef8c0cf4fc71c141acbef542a1b0f90095f485319d98603
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123465572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23495bcf619fe80e0df2d9ba0d3e0e620c4531aaf7154f152d41be5264dd2ed3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:20 GMT
ADD file:b2ee7e73ad4207feb437f92888b1a73e57515c82fc8325c4604d21a39771e52f in / 
# Wed, 26 Jan 2022 01:45:21 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:39:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:39:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:248f9d803d87b1b0a005a24c98133b989ced8e0b664be38cb600b683c4593899`  
		Last Modified: Wed, 26 Jan 2022 02:02:42 GMT  
		Size: 53.3 MB (53255788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc4178c3c07ea158cad18d885ec03af227796d71c4a004c8f15b307cc4de474`  
		Last Modified: Wed, 26 Jan 2022 03:01:01 GMT  
		Size: 5.2 MB (5174902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c0983cc859431bb8e8296bbc443587cef8bf5f35a9b346102ec3018f68c610`  
		Last Modified: Wed, 26 Jan 2022 03:01:03 GMT  
		Size: 10.6 MB (10582966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f1901338eb48d32091b355f97f4e8453becf07e5c6f3213246056f8f8c150b`  
		Last Modified: Wed, 26 Jan 2022 03:01:58 GMT  
		Size: 54.5 MB (54451916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d45a4c2d3786eb4c9d6f0b8fe126088127312617d5118dcdf36f12e554f450ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118491046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1250a43185c0f63d7d1144764fbd0d5abe7a1ddc9ffbac2821ac7202bfbae69d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:42 GMT
ADD file:25bd7c90ec9cba9155b5f5e4b8ba10eee0a84413efe182bfd8e270eec1783ca2 in / 
# Wed, 26 Jan 2022 01:45:43 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:45:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:45:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:46:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8beb160c955a6211ac47cc7f90ad3b37999d7da6c9b2f0d32e82d6ac9bb4e6a3`  
		Last Modified: Wed, 26 Jan 2022 02:02:50 GMT  
		Size: 50.9 MB (50897789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5033ef8051fa00849de7e1029124d977fce14e2255ef3ea2e9a0aa226e20a793`  
		Last Modified: Wed, 26 Jan 2022 17:09:44 GMT  
		Size: 5.0 MB (5035338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2221dacf46091a2f23a799af18530570a3c4d219f9d87d052eb48e5982c95d9`  
		Last Modified: Wed, 26 Jan 2022 17:09:46 GMT  
		Size: 10.2 MB (10241510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1f76ba35e51e63fcba8c49e3f3d26df6cf84550a69e9a8be7657bff2df3d43`  
		Last Modified: Wed, 26 Jan 2022 17:10:35 GMT  
		Size: 52.3 MB (52316409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c5bbf76ce5ad967bb24f62647a099185fd521ead9889f64c4e72b09b8e38a2db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127550981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b19105392f83865a275f1e6ec729e0ee4ebbd96a2e757e825abd5df9868bc6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:52 GMT
ADD file:b374f2870285b974edf3ed21e9bcab7b86f3d5f58f504052e4ef7507affd730e in / 
# Wed, 26 Jan 2022 01:43:54 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:16:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:16:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:16:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3c162c40f334c8be5b3a873f3af9fdbb3e46d36b02232496f08adc78fd0d1197`  
		Last Modified: Wed, 26 Jan 2022 01:51:38 GMT  
		Size: 54.8 MB (54776771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e5527738d1213690712a506bdfb6a4e4e53f00abc3a857f27e46783342a012`  
		Last Modified: Wed, 26 Jan 2022 02:26:12 GMT  
		Size: 5.3 MB (5263075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb344bcecb1f1e4eb7e0b7d7ceb695b290ff4e82c3967bc1c646a8c98de6d21`  
		Last Modified: Wed, 26 Jan 2022 02:26:13 GMT  
		Size: 10.7 MB (10676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3064c5c0474d687b691ad542db19a5af822c25a6bb02dcbdc584dcf2f73154a5`  
		Last Modified: Wed, 26 Jan 2022 02:26:33 GMT  
		Size: 56.8 MB (56834268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c843ef7d6a89262170b031e2895ec217a193b67591073bc25c86f3be8ed2e909
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131764999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c54daac1d14d7f79df7488f16b4e7f261470268b8676c36ddc3955f8f1779da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:51 GMT
ADD file:da0be8aacf1ce5f6b8eac72cc37cf866a1f42436b73a7491a048fc296e2aec59 in / 
# Wed, 26 Jan 2022 01:41:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:19:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:19:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:20:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9befaf96f69d02ac54d26fdd6569c9b6bb607e4566ebcdba828f8df0ed688997`  
		Last Modified: Wed, 26 Jan 2022 01:52:27 GMT  
		Size: 56.9 MB (56852445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1205a9ac4da466a85715ecf930f05eece9a89e5b6f512222898eefe087f5697`  
		Last Modified: Wed, 26 Jan 2022 02:31:45 GMT  
		Size: 5.4 MB (5407567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59261fa94d22670274f83195f55b41969e923771145bb95d95eee75fd629f932`  
		Last Modified: Wed, 26 Jan 2022 02:31:46 GMT  
		Size: 11.3 MB (11307649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11174d44c83ac43ad98b9ef06e4e3c5a9d22a22478837f0bcb6e56b78fa74d82`  
		Last Modified: Wed, 26 Jan 2022 02:32:18 GMT  
		Size: 58.2 MB (58197338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ce4b6785e79ebc74b74c7abd3ecc41024b65ab0f0e57eb721a96c28d297c93c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126227400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebb4c51e03f6b4b0d0f01ba58ee73c6ba807e92d2942fc5a0b7ae5ef1421a0a2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:58 GMT
ADD file:ff5cb17f112000b0283048e51a31c66fa6d3b7b5c73ebbb9e407d66773bd71dd in / 
# Wed, 26 Jan 2022 01:44:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:30:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:31:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:780a90a74dc946c86fcaf8ad99094385c527418934e8729eb8e19bd129202058`  
		Last Modified: Wed, 26 Jan 2022 01:54:46 GMT  
		Size: 54.5 MB (54487249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28747c788a9fd6c864f18d440188468cf9eadd01d3170b173b0dcabaffd1dc0c`  
		Last Modified: Wed, 26 Jan 2022 02:44:18 GMT  
		Size: 5.2 MB (5231642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e77450002c767308f9f932c83fde37fdf6742b761b14caad928f47ea3c8735f`  
		Last Modified: Wed, 26 Jan 2022 02:44:21 GMT  
		Size: 10.9 MB (10875142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6aadb0cded3445b65cafacd82549fdac52529a699b3223b960634edbc065aaf`  
		Last Modified: Wed, 26 Jan 2022 02:45:11 GMT  
		Size: 55.6 MB (55633367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c2971c9405c0dce64d7b47e85aa1314e6e70196f3d2f74c3910714c99a9ffc02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138904302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eee105c7b48a243e12df5d5ca7c6d8d096378558d969340da190fc0654666b8c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:50 GMT
ADD file:00619ac2b9b09af1ef0989fac7a97e811d92f85cef55887a843850c6edd6397d in / 
# Wed, 26 Jan 2022 01:48:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:58:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:59:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 03:00:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:207334870a9e08012db59a768343c68c9297e1123cfd3f49c878d325443196c9`  
		Last Modified: Wed, 26 Jan 2022 02:01:42 GMT  
		Size: 60.2 MB (60197594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e44ef395f05a799994decb77ffb1782c89a4c0282be793f404418d1a7f1d81a`  
		Last Modified: Wed, 26 Jan 2022 03:25:17 GMT  
		Size: 5.5 MB (5540064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f233b52a0118c53ec4e4fcbf2d80e0f1a054746b47ff133ba2e3c92eb1246992`  
		Last Modified: Wed, 26 Jan 2022 03:25:16 GMT  
		Size: 11.7 MB (11693400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f445939acd54056bc3389536f9954772ff534bdffa069800f03bfe155736b47`  
		Last Modified: Wed, 26 Jan 2022 03:26:24 GMT  
		Size: 61.5 MB (61473244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:6b91da13d7013eab079224fbd7fa095000006ed0df6803da49afa74fde9ce696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119768333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea75dc836ca3dcd73c98a3517af8d39cdd357c584e767e7f30a3882d930c52a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:14:08 GMT
ADD file:1dc8a81ea9c954e594eb32623a82cdfb528586b569a915ba8f70a49f68a6f7fd in / 
# Tue, 21 Dec 2021 02:14:10 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6b741955e06623f1924320507da1630323c4cf1d6489febc99917464e765860`  
		Last Modified: Tue, 21 Dec 2021 02:30:31 GMT  
		Size: 51.5 MB (51541457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91689f9aadadd96fe4e4ad4ed92ff1cb6a48034aedc9f41e14d54cf85bcdd039`  
		Last Modified: Tue, 21 Dec 2021 03:34:04 GMT  
		Size: 5.1 MB (5089016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a290be0dbc2a1d1f5f12db96d9dc0949f33b55d33712a23f37c71cb89606a3`  
		Last Modified: Tue, 21 Dec 2021 03:34:07 GMT  
		Size: 10.3 MB (10320854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44222df82131b4d925c2f594e50c018b1fb6d67154b22de79d99eb4cd4a356c9`  
		Last Modified: Tue, 21 Dec 2021 03:36:17 GMT  
		Size: 52.8 MB (52817006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b4adcf2e69464bee8724fa01dfc0e685bf3807fbf49f4bf37095534b69431df3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126317703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7e49f1bbf169c9511204574516b7987e34337c021d472b09c4930623556f9f0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:22 GMT
ADD file:3bad388a0bccdbe60c35b9f2f185f24531da6894d5fbaaef83c17aaaf447084d in / 
# Wed, 26 Jan 2022 01:42:25 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:11:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:018136a50defba2fd8fcf9a0ff234cc3971c8e2e29eaaea1a3db05b950df25a2`  
		Last Modified: Wed, 26 Jan 2022 01:48:18 GMT  
		Size: 54.1 MB (54089891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b646642536852c2c78a0d07f56fe415018ecf441c1ff4bb1f3672347e0a16d0`  
		Last Modified: Wed, 26 Jan 2022 02:20:11 GMT  
		Size: 5.3 MB (5254889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716bdea6cf2de7b0ea754b38c3e71201e96482b618ecfe5cdd22d50c44f2853`  
		Last Modified: Wed, 26 Jan 2022 02:20:11 GMT  
		Size: 10.8 MB (10807427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dbff4fde8ad04d5d26795083faa946b6421edd89122c7b1df66bf7226604bf`  
		Last Modified: Wed, 26 Jan 2022 02:20:27 GMT  
		Size: 56.2 MB (56165496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
