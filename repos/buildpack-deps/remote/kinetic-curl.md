## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:f66a1c64c8016d63b3a16e0842346dd818c9a90e4f6d773d1f5448505e902365
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ea9a4495f81bc39c024a6822db560f533e9e0cb8d43734db0ec3d2f320209c3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37800306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8204d4b0a65cab6e872261ed07232a618a9dce3106e4450b0a0fbbc9f2da8893`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:02 GMT
ADD file:e5fa8bc7f766f2ed38c381684cb1db20880e853d3767fb3c11d7c2c82f166df6 in / 
# Tue, 02 Aug 2022 01:31:02 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:11:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:11:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:90b96841878b7af8ea3a64515404538ce0332b459991609eb863be5db84a3470`  
		Last Modified: Tue, 02 Aug 2022 01:32:34 GMT  
		Size: 27.4 MB (27444732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d0dd055e4367f30e890d117b6f1ffd6db44dd0aed3d102fe5eff81ef9efcb3`  
		Last Modified: Tue, 02 Aug 2022 02:25:19 GMT  
		Size: 6.8 MB (6788538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7b9cc450b3fe5f68921cb876bdc2ae34b4e682ac83c2ef0a9afc63500440f1`  
		Last Modified: Tue, 02 Aug 2022 02:25:18 GMT  
		Size: 3.6 MB (3567036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9b85bb80fdffb064474fb1505988584cc2962e0070e5f35f08fe58ab5f498f17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34512271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fea3f676032be24f5daaf4e9824da2d7e0aa8a0907d7fda8e82b01cd4860b3b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:41:08 GMT
ADD file:66e6471f52fc58fc2800d34f1d39716910c1cda3611b70b14120742c855b63ad in / 
# Tue, 02 Aug 2022 01:41:09 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:01:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:01:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4f8bc5dc03fab2ee54b70f6218aaaa0c6cd0f00b7df0e688df71d48899d1633c`  
		Last Modified: Tue, 02 Aug 2022 01:43:57 GMT  
		Size: 24.8 MB (24813035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0730d1b5a4dded6f7fae7ef8804e621785ca732706a3a9cfcd18833cf802fad`  
		Last Modified: Tue, 02 Aug 2022 02:17:55 GMT  
		Size: 6.0 MB (5975718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783bb70087bc78639e7d81451739990ad377e2a52f9f4dbd7ff7beca3a622906`  
		Last Modified: Tue, 02 Aug 2022 02:17:54 GMT  
		Size: 3.7 MB (3723518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fa7e8d2326a74eef695777015fd08f2cd2f0d29f9a81c2dd3199ad74fd0f17a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35536375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a42c2f889df2244b5551aefd3782eaaba7a4502549af92583a7965ed6de88d2e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:08 GMT
ADD file:9a13d2dd4ecc4e3136c25a7b16372d77ee8ccfb9b3fcafd78af5797485ffb038 in / 
# Tue, 02 Aug 2022 01:19:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:38:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:39:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f229a80be8f0f33867b5a29c230954f11922f0e641aff2a6c16048c533bf5290`  
		Last Modified: Tue, 02 Aug 2022 01:21:12 GMT  
		Size: 25.6 MB (25575171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fa5256bba7c1c373d0a1ef1a0465e7994cf5726371518dc47bc17dde7bc45b`  
		Last Modified: Tue, 02 Aug 2022 01:51:54 GMT  
		Size: 6.6 MB (6622247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a514ca1576757eb70513da350b92d860ca64561744d13659787f0224196f53`  
		Last Modified: Tue, 02 Aug 2022 01:51:54 GMT  
		Size: 3.3 MB (3338957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a1779ba852a8296487662a4b702a97e5607c12e1adeaca781bb671e4520a4cbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45463138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff41536c14becf51e9c0b888099987d1822c9d33264b16cdc6beb86bbbbdaa59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:47:11 GMT
ADD file:94cf6534c6b66a46a13144239fd0bba4180772804f5826d12fd030c1199457bb in / 
# Tue, 07 Jun 2022 05:47:14 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 23:25:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 23:26:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d9ce8aa65c6465c42b081a5642262f289b2db6cfd58b6e49f7f2c24742205c2c`  
		Last Modified: Tue, 07 Jun 2022 05:50:20 GMT  
		Size: 32.1 MB (32131305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a03c5d4a4a30095b5986889adae05bbb0933ce7e48e115e1b7fd75ae323e8e`  
		Last Modified: Tue, 26 Jul 2022 23:58:38 GMT  
		Size: 7.8 MB (7802631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96d280d0e21317e7cdab167420493ea718b004c6e2a490a3e7e242cb0db32`  
		Last Modified: Tue, 26 Jul 2022 23:58:38 GMT  
		Size: 5.5 MB (5529202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c56a99d1010d118ce31bd21a5629430290fb055f9653357ea86663253502b41c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35176975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0923f700014ab1e1769c493d806afc0624323a9e87c7b536394b879cc0ab34d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 18:21:26 GMT
ADD file:7360bdaa4ea5ec8b4eb9b93f92717ed4fb377c6910368b3f1af3f2524989f28c in / 
# Mon, 06 Jun 2022 18:21:27 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 19:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:46:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1df12f21536751a4a4297772577c4c96de0f5030dfb5243599bd956eca3d066a`  
		Last Modified: Mon, 06 Jun 2022 18:45:02 GMT  
		Size: 25.4 MB (25435182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665f6f3ab1186a3216e891819468ac8dc7d533ab721c7be256ba7c56bcfc03dd`  
		Last Modified: Mon, 06 Jun 2022 20:38:03 GMT  
		Size: 6.0 MB (5960974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fcae399ce23346d8006049bedfc5c045fcd5e2575d2549db9d528ed359ac49`  
		Last Modified: Mon, 06 Jun 2022 20:37:59 GMT  
		Size: 3.8 MB (3780819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1cd4837220dd0a4f85f14d7ee17b62a638d56056040b073a5471407ebc9a3836
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35901531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ac878a01b3de4ab026adb149927e09c3db0ab1773ebabf870ed1071c627abaf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:28 GMT
ADD file:6110741104bb6cdab4d1f236e0e14d83788d0d9be2c117cc21b818cbe53bb7c1 in / 
# Tue, 02 Aug 2022 01:02:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:28:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:91b26e5129898f349569cdb5e70f8a6e3046baf255fc1b62684edbcb5f7f47bf`  
		Last Modified: Tue, 02 Aug 2022 01:04:08 GMT  
		Size: 25.9 MB (25944242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4afb051b7b1df235b2c41c69ce633d0f3026bc2d13a7ecb55d0cb483443d931`  
		Last Modified: Tue, 02 Aug 2022 01:40:23 GMT  
		Size: 6.5 MB (6476893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c5e4c7745db385f92256fe54757ac7d96ef0485584e1ba21d24b2b7d6ad7e1`  
		Last Modified: Tue, 02 Aug 2022 01:40:22 GMT  
		Size: 3.5 MB (3480396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
