## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:e22d0812565a3ae27b4c0b4c79db1bec96c5cb6360bb17d2e4eaf8d827e0a44a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5a45d64f39849ff1d5c10bfbc6da97c20f72a28dc45349900913e2927b2cd9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71785755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20b5f544bc4e1e87120699d838ed693db78e7a0d77a59620044bb1d40e422a7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:09 GMT
ADD file:15e5b0a35c4fc7a5ae0bf08f713bde738d2cfb06a30b8bd5780fabafb91d934c in / 
# Tue, 21 Dec 2021 01:22:10 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:50:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:50:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9aa4f47c6909274e4d7f0b2429a7ad24598b19c01da78245a16a3176f9acf847`  
		Last Modified: Tue, 21 Dec 2021 01:26:44 GMT  
		Size: 55.6 MB (55598801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f71e2132b1cfc0df72e7252fbbc759f38ec76718cbb194e3f3abae59f6c6f7`  
		Last Modified: Tue, 21 Dec 2021 02:00:06 GMT  
		Size: 5.3 MB (5282859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f2c25fefbc6f35b9aa1d2da6608ac2eca9de0a624ef3624ea94b11c7ed3db4`  
		Last Modified: Tue, 21 Dec 2021 02:00:06 GMT  
		Size: 10.9 MB (10904095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cce513c1ad2a19b051d052e0860f76f867aac45cf84ef4a7608788481c279d9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68823963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69cbc5575a3e9e3069d1498b95a52a83f47567a82bc563d325893b9c62126c4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:00 GMT
ADD file:565dc0a92c6ce86500c032d7c7e8112f62771ff3bac3aa84192e8309ae7acbba in / 
# Thu, 02 Dec 2021 02:49:03 GMT
CMD ["bash"]
# Fri, 10 Dec 2021 21:49:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Dec 2021 21:49:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:92dd04f71649984a91d8241840b2fa0a06cee72bebcd6503ece93ae1b5f47d07`  
		Last Modified: Thu, 02 Dec 2021 03:07:38 GMT  
		Size: 53.0 MB (53031153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034d98e044e9e53481f8d4d8abf3a1c951af6e2e0302f2d5c7b0bafe2d4ef536`  
		Last Modified: Fri, 10 Dec 2021 21:58:02 GMT  
		Size: 5.2 MB (5181891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfbba8655504d3ed9b02abdf2cb4d87d6795189ed0afd4f34e9f46363bebf`  
		Last Modified: Fri, 10 Dec 2021 21:58:04 GMT  
		Size: 10.6 MB (10610919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6153de1ec63e62cf418b13862bbc92515e271c492821f012023992e60f574924
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65962827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c750604612e6dc6eb5268a0ffb44f2cd5d2a3e01bd1b3704b6eb89a3ecdf4d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:03:39 GMT
ADD file:bd5233b326b625660d820fa962832e6c5413ff9a56f64a6f072b9a9adfc545b2 in / 
# Thu, 02 Dec 2021 09:03:40 GMT
CMD ["bash"]
# Fri, 10 Dec 2021 21:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Dec 2021 21:58:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4dcb906f06af542b010e092a9a4d4ad8ccb110debf57beb0d4ded9baa51b82a1`  
		Last Modified: Thu, 02 Dec 2021 09:18:59 GMT  
		Size: 50.7 MB (50667986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6290470e339a2322159fc965896cd31eecd849410e2d52a8d8ecfd35f27f39`  
		Last Modified: Fri, 10 Dec 2021 22:10:56 GMT  
		Size: 5.0 MB (5041382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffd92cf9cc4dbaae187824ff4063b4fb6ee16274347a41c15b4c1609885dcfd`  
		Last Modified: Fri, 10 Dec 2021 22:10:58 GMT  
		Size: 10.3 MB (10253459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:92dc4818a14cb5507e90c2b1d1993ece5abae3e306427fbef7b4d2769fecded7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70549254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1682ffce1225f37ba827f8bc954cbca134fe20a72572a7e490dfdc8e07ef74b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:41:45 GMT
ADD file:c64482c2e0b0935b000b024e468499d2586b78ca5c64b035ded7ce33f1dabe14 in / 
# Tue, 21 Dec 2021 01:41:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:10:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:10:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be902f523b4c4ddf53ea157e340cd7ce836ec2a0952d6f18602467352524e312`  
		Last Modified: Tue, 21 Dec 2021 01:47:42 GMT  
		Size: 54.6 MB (54598073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae3b1dd188183d78f548c40b842d6abda988dc1e02042a8d2fbba1292db6225`  
		Last Modified: Tue, 21 Dec 2021 02:21:21 GMT  
		Size: 5.3 MB (5271381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d762390d417c63f26301db70b2fc0b6cbfb2a625b710902a4efa39a4fbe7eeac`  
		Last Modified: Tue, 21 Dec 2021 02:21:21 GMT  
		Size: 10.7 MB (10679800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d82db7f0f4ec19dfcfa906d32310f92f3a10c46bfce45af424d5395d21cb62a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73358733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91524aec366da31958a0d251d1611a4aa6d32e07cc448f51e44e3d5ec7b0c62e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:06 GMT
ADD file:f5394800b665e61b6f319d6dffbccd66c1172d4e9fd1db6ba962ef5aa177c353 in / 
# Tue, 21 Dec 2021 01:39:06 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:11:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:75388d3fd5f848339be12f5cd41cdf79effd086f4656396bfbac934b7f1f715c`  
		Last Modified: Tue, 21 Dec 2021 01:47:16 GMT  
		Size: 56.7 MB (56658883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de7e33a377d91eac773d98f83f6ca3f85f496a95ef1607a2f5af89fb4471391`  
		Last Modified: Tue, 21 Dec 2021 02:24:06 GMT  
		Size: 5.4 MB (5414374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4180045f386d2f79d4770aa88797a1fda448758575d57afc6ea4e781dc548b5c`  
		Last Modified: Tue, 21 Dec 2021 02:24:07 GMT  
		Size: 11.3 MB (11285476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2627cd9cb56bf2d909eb64d9ce8c5868c0e72f8116138d4621973e72879d142c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70416331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64327a029e3fdd09da3b6d3af5a084a7a12adfe32af016e90b31fd939214a194`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:07:51 GMT
ADD file:2b78b392bcc6daef3d9c93dcae4adf8b84cac89c57ed08bd43854d23774078d6 in / 
# Thu, 02 Dec 2021 03:07:52 GMT
CMD ["bash"]
# Fri, 10 Dec 2021 22:07:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Dec 2021 22:08:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8c4a35c3e932252ccb2418c1bc14531f11d21f13ba131d0a52cd9cb690dc9623`  
		Last Modified: Thu, 02 Dec 2021 03:15:53 GMT  
		Size: 54.3 MB (54269592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5382fc82d142248068645a004ecdcba9b86008e8e6d072fb2a8b85524a38c87c`  
		Last Modified: Fri, 10 Dec 2021 22:12:49 GMT  
		Size: 5.2 MB (5239618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d5f987669cd4335e12d30a8b21fb2532368af6d0867a4749dc32ef5e0350f`  
		Last Modified: Fri, 10 Dec 2021 22:12:51 GMT  
		Size: 10.9 MB (10907121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d0f585cbd76626ab15a058b6a72955c67e9d8b36eb72d916c275dd6bbbb52492
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77053689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9a3661898e08c4bee28bb2bf82591dbff1dea13f2647bd355275d72bf5a247e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:51 GMT
ADD file:b1221d684becfd74b167e24d774eb6099d264be14e0abd56599cb6a39c9eed74 in / 
# Thu, 02 Dec 2021 07:20:00 GMT
CMD ["bash"]
# Fri, 10 Dec 2021 22:17:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Dec 2021 22:18:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5ad94a9a32e9daafdd41e8b09d1671e7fd6b6d7cff42957db5b36cf5fe8276d1`  
		Last Modified: Thu, 02 Dec 2021 07:29:36 GMT  
		Size: 59.9 MB (59851370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190a5d1490ffcf131ea963f82913c2ec2d57ee0b6741316c88d37d687342d657`  
		Last Modified: Fri, 10 Dec 2021 22:39:49 GMT  
		Size: 5.5 MB (5543063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be29388656987e957ca7f48c588ec4c6cd00a8d2d9eee951d82efdbe540d681`  
		Last Modified: Fri, 10 Dec 2021 22:39:49 GMT  
		Size: 11.7 MB (11659256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4a636643e4a7d941b2170756253bd99782ed012838ffc23b458dd80c37f24721
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69948338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e6a1003d0507e54e2e71410fc1ed871d3177e540e8c848b1e556dbb4464a554`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:41:36 GMT
ADD file:c9626c75e4b53a0e71f37a2a3df45699d003ae102e7e3eedc97afe7897f82180 in / 
# Tue, 21 Dec 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:07:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:07:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:341c5a56ba0f7b7f22f0613addb31ee3342e410686dda8753a049d0bd1f319f3`  
		Last Modified: Tue, 21 Dec 2021 01:47:23 GMT  
		Size: 53.9 MB (53888441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8be60271199953262ee02a4148a07af9a66fa017104d2d03d65d92956150fe8`  
		Last Modified: Tue, 21 Dec 2021 02:16:46 GMT  
		Size: 5.3 MB (5263047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100220edd1ab3877c378dcbe4658541db3dcee1ff143d2e1e5b5d75d67380a9b`  
		Last Modified: Tue, 21 Dec 2021 02:16:47 GMT  
		Size: 10.8 MB (10796850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
