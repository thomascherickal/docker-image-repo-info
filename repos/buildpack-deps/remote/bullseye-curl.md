## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:a6e143c4b96f8eee7a0a7d1e82ff8e11dc4c1dd07af59746dc1da5c000c71995
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c3b2fa775aa81299b26a50864a0317229aadcbd87fae72a73c00c83d95cb35e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72190361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1e8d15464b6d5d487b9593c0f5787e40a8b580ae69f361a093b610bfc26639`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:09 GMT
ADD file:730ef8e3327df644cd47994a561a489bfcce5da8103cc8eb34e67321a36df2ba in / 
# Tue, 12 Jan 2021 00:32:09 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:55:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b802c2c29a7757c7475a0b343a18a46b6b27dde9e3fb6b4db61c68ea197b51d2`  
		Last Modified: Tue, 12 Jan 2021 00:38:04 GMT  
		Size: 53.6 MB (53566443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd06bfac0a19b28c6511794acccc260657d53a299701a82ec9fcafe465089350`  
		Last Modified: Tue, 12 Jan 2021 04:04:36 GMT  
		Size: 8.0 MB (7974792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d97704dcad5e05944cbac93df8fdf452cb71e698fd44004184391a44e8787c`  
		Last Modified: Tue, 12 Jan 2021 04:04:36 GMT  
		Size: 10.6 MB (10649126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ea8258eb0f46cee6ee6e376af9a9d6abd3fc423d76e9577300acecfd6ad2c1b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69351032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c588dbf53ef7521f0529e62869b4460167c6754d3d352a621ea9ce7065e56b21`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:50:29 GMT
ADD file:d4da31b3c934d9b6c8328e7951f06cec1babe1f9674a7a3ee2e87670575ff01c in / 
# Tue, 12 Jan 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f9810833d48e3d19cbfbfb8871ba282d104d5bcfae1b19c0c003f9811dbe7c4c`  
		Last Modified: Tue, 12 Jan 2021 00:58:53 GMT  
		Size: 51.5 MB (51487444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257fe5697f52f59aa0dbdede36db8adf4c0796905b3388832de43ac1e4ab97d`  
		Last Modified: Tue, 12 Jan 2021 01:41:45 GMT  
		Size: 7.5 MB (7527914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c59bb7c72bcd7ff3df84ab37209a928574816146c37f0808619c4b5a6dde4a1`  
		Last Modified: Tue, 12 Jan 2021 01:41:45 GMT  
		Size: 10.3 MB (10335674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a6eb0fadb0bef5514f4f004575e1216dabe7f7d926cd42dacae124aeb512ccd0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66399716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91263701c62ae3a86f4732fc1a5c5feb04184781eda4728fb624f30c788d752d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 11 Jan 2021 23:59:52 GMT
ADD file:ad9ce4dd05291eba636daae5f0b9de510927734ac26dcca6940d93e88b5c5330 in / 
# Mon, 11 Jan 2021 23:59:54 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:11:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:11:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4ecb0a075e68a9a1a4b7394123b05b2811afa9bc0a23170e2e6c42d5ee19a7ac`  
		Last Modified: Tue, 12 Jan 2021 00:09:56 GMT  
		Size: 49.2 MB (49159573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dea32ec53c55b5a19d9fb093241be9ba6e2fe2fd55963111e57d39b0973f01c`  
		Last Modified: Tue, 12 Jan 2021 01:27:54 GMT  
		Size: 7.3 MB (7265094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b285ad78deb9119d75d41a2decc62fd9676078225d860eec32d20835fa7fb`  
		Last Modified: Tue, 12 Jan 2021 01:27:54 GMT  
		Size: 10.0 MB (9975049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:43d4736915d4b66b791ef4dff3d31645e20816250f5d18a3488cb6a6d678a701
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70923298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f4fd9f3dd5c3e2442efc4b43b90be7e813074e1ce15a875ce5ae7d95b235ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:49 GMT
ADD file:0700c58361c6ae34d399d7ca2a5a6f509980a496c07d319f7455d86b483e7f25 in / 
# Tue, 12 Jan 2021 00:39:56 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:19:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:20:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d1e62204d5e176f9e5ef453b346203f7bda9e22ed810a0a4e2c14548d7cc3afe`  
		Last Modified: Tue, 12 Jan 2021 00:50:17 GMT  
		Size: 52.4 MB (52428437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f37b86a934fe39fb5aebaff30977af7d0075b2eeb06b1b794582ae2566dff1`  
		Last Modified: Tue, 12 Jan 2021 01:36:53 GMT  
		Size: 7.8 MB (7840062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0908ecaa573834d3855dd61a0aabaf6565245ab200624d87774802a93f1b2dea`  
		Last Modified: Tue, 12 Jan 2021 01:36:54 GMT  
		Size: 10.7 MB (10654799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0c0dde90b4da711fa6cc88f35f5630659fad7f87bc839f12d249d9fcb987cf1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73807720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b5997494b72775bfad0059cf2bd13700bb96a4c820f8f2739ed8eb73f26d24`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:38:50 GMT
ADD file:5bf2c8336f63e88ae7e3d1d6804439d7f6a54937823f8e72b84f8bc95c97391e in / 
# Tue, 12 Jan 2021 00:38:50 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:15:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:15:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a8d8d38d6122a88724bab503447c48e782190ba13d75634b2b651e6dbe0a0225`  
		Last Modified: Tue, 12 Jan 2021 00:45:03 GMT  
		Size: 54.6 MB (54617930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c3a2f57bfbcccfb355c377855cb08176af609e0a121945636c2af1f19b110`  
		Last Modified: Tue, 12 Jan 2021 03:29:40 GMT  
		Size: 8.2 MB (8157573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e0211a7714f69b0754581dbc4d3b367733f5113d0b6a49c72623b3327621b4`  
		Last Modified: Tue, 12 Jan 2021 03:29:40 GMT  
		Size: 11.0 MB (11032217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ae3960e65ddaa86d1d494e5b47f6ea7a197a80903c9ffbebcf03d002e0bcc8e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70414851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5560db536fa1a7b44a1c4f9c4ac634401272c0293aa958e468793c1aa8e7ca2a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 01:15:12 GMT
ADD file:171276d9060030f06df201450c4356d6449f4c6a905d02db7f2371f7ed26b34d in / 
# Tue, 12 Jan 2021 01:15:13 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:45:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:45:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cdc62d8dca2f8e7c324fa9f4efc40193ada4c98be9ca6b3f1388ad903e4bd5d9`  
		Last Modified: Tue, 12 Jan 2021 01:20:56 GMT  
		Size: 52.3 MB (52264790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60b87fc90acd9bd7359cfb81de768ce7f4cdc0821db3ed523142fe855433832`  
		Last Modified: Tue, 12 Jan 2021 01:58:49 GMT  
		Size: 7.5 MB (7492735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6084ef3498948096f602b4aac1a0fb7a2dbaa7d5d751897ddec139d2cebb08f`  
		Last Modified: Tue, 12 Jan 2021 01:58:51 GMT  
		Size: 10.7 MB (10657326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:395e3354a94259806ac798908af6dc02791e1f6eb0f555f0f36e2608ead4cff2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77415262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e53a0af5f4fa4668472028f5f823c4da07c357e467f66dbe2cbaa4a04a20fb5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:23:03 GMT
ADD file:840490bff9a0b2cb1e20599d893c1160f6884327f51294479567e5d43f91b885 in / 
# Tue, 12 Jan 2021 00:23:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:39:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9d21ce86f5496c36ba2ba289acb977a3b160c6c56fb257c10e3adb8b55164a16`  
		Last Modified: Tue, 12 Jan 2021 00:32:24 GMT  
		Size: 57.6 MB (57562164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d42b61558772eb59064c0ebad8029e0e7524bf865c29218b048871cd3e43fe7`  
		Last Modified: Tue, 12 Jan 2021 02:37:14 GMT  
		Size: 8.4 MB (8431230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663cfe2e2cfc28477e509f0e7aaffd4159d2f37157b32a7327bb6f43a7508ac4`  
		Last Modified: Tue, 12 Jan 2021 02:37:17 GMT  
		Size: 11.4 MB (11421868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:db64377208b56bcdb13e9fbc597e03604218318de076730e27676022c27a82a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70283366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2142411addc51ea4c906ecc47af9ab1e2e2d418309f3c3c69f57b178973d58`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:41 GMT
ADD file:5007beabc318acc6a33d879e231105324ef7801fb709d3d69813b180e883d64f in / 
# Tue, 12 Jan 2021 00:41:44 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:07:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f1b527eede6bdcb4cce85e897c3a92fbf04bb476403758d3b535dbf6e388d192`  
		Last Modified: Tue, 12 Jan 2021 00:45:27 GMT  
		Size: 52.1 MB (52107904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f7f4dc3450e7b31e01a1746ba85df290d5b698d495c8ab448923393956e52c`  
		Last Modified: Tue, 12 Jan 2021 02:16:42 GMT  
		Size: 7.6 MB (7649499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945c37e35656a95430c56e2a6bb0a416252a37130eca65d1f3beee38efee696e`  
		Last Modified: Tue, 12 Jan 2021 02:16:42 GMT  
		Size: 10.5 MB (10525963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
