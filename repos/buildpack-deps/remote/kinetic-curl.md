## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:bebb72cc0017ada08900d2a46a1ffb311cf682d7232bd1f5843c2def438a55af
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
$ docker pull buildpack-deps@sha256:ea6b96da9df04e5c6170ccefc1a7a45e42c610401d4004132b7b0f57f2327dc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37708867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef9b94b0b8f97abb9935245038aeb2e54ec157f9bc73aec0d4f87c28bc8f3e4`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:33 GMT
ADD file:440048faae869c09f5819655d93c479ac0282dace791dc6077f035c8481f45b8 in / 
# Mon, 06 Jun 2022 22:21:33 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:20:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:415d72858c745ad20ae2769e6ba46966432d24b0cb79e2ebcb65280ce8248a31`  
		Last Modified: Mon, 06 Jun 2022 22:23:23 GMT  
		Size: 27.3 MB (27347519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd927167c75021e878fd8d0927d91affc71fc2a4e099b9c4fbab2d9230f68492`  
		Last Modified: Tue, 07 Jun 2022 02:28:12 GMT  
		Size: 6.8 MB (6796121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5f9c7747d58c8108a20268f5d5b0603de8d390dfcb3d66f0bb462ed4757290`  
		Last Modified: Tue, 07 Jun 2022 02:28:12 GMT  
		Size: 3.6 MB (3565227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:be2423e73a2144546c5cf2be3d61619cd494cc06b40a4db352f7409fe3a7275b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34366175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4f05f35ac7013106a520a4dbe6d15d96bf4f1319609e2ad7ae326283ce2063`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:52:00 GMT
ADD file:243d0f716fbef71d7d9cc76cf15c0b298f5b3460b6533ab2a8e88b0d618dc144 in / 
# Tue, 07 Jun 2022 05:52:01 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:10:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:88f853be8de2fbdcfad5b9be55e0f368887c6cad36efaf35cc75b81a8ecd9841`  
		Last Modified: Tue, 07 Jun 2022 05:56:37 GMT  
		Size: 24.7 MB (24676229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8309bc9e188c93b03413a75296e80a55a55d4c4cba09aa7a59044c6b2cdb680`  
		Last Modified: Tue, 07 Jun 2022 09:30:23 GMT  
		Size: 6.0 MB (5975769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc52d4a1356b55b3c78029b3cc039697533033c4bc0d17a13f479f27eb467f5c`  
		Last Modified: Tue, 07 Jun 2022 09:30:21 GMT  
		Size: 3.7 MB (3714177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5a66735fe6ae53b5b341de1979390884892a6c128a67471be7de856d6df22939
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35409549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5504ccfd863d3b054e2a3717978453eb6da69db027d1fd7daa1b8a9ade148ef8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:41 GMT
ADD file:436ba9358911a376f8184a243173151b7b2ef9c66c14edfcd003f07c65a22f1c in / 
# Tue, 07 Jun 2022 01:25:41 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:50:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:46465228a6c0c2b6f599636b0a2e73f8b6954a9be77e8b309c72783a93fcb092`  
		Last Modified: Tue, 07 Jun 2022 01:28:07 GMT  
		Size: 25.5 MB (25459707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1173afc37d77836d87cb4f01d6e5b5960d43aab0605773475fef37da1902d856`  
		Last Modified: Tue, 07 Jun 2022 04:58:28 GMT  
		Size: 6.6 MB (6625122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8db28861a6be1cb9b6df04a34d51a5f92117bf390da3935a0260bd09e93e1c`  
		Last Modified: Tue, 07 Jun 2022 04:58:27 GMT  
		Size: 3.3 MB (3324720 bytes)  
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
$ docker pull buildpack-deps@sha256:8d5b0f2d5819fcce49f94ff26e43c5da3cce4d553d51479848c85bfb72d24ea1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35817639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d09eb8d22fe2283603892e79df42cc8fac676ddfef3fba9ad69b957c1e9cfe6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:06:01 GMT
ADD file:73b8105e3f6b064f2f8039d2102cfa51946b6b268f19a0e6a348fa49cd0ed2de in / 
# Tue, 07 Jun 2022 04:06:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:00:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:94e4f8254e7672b5bdebe620b1922baa63fd40872238ee59c3f48a8d9485d43a`  
		Last Modified: Tue, 07 Jun 2022 04:08:31 GMT  
		Size: 25.9 MB (25857245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c529509938b721f50f025e2e2969140aa4cbdae823eb10b1c6b51389f52f11f5`  
		Last Modified: Tue, 07 Jun 2022 06:09:53 GMT  
		Size: 6.5 MB (6482918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dacc17ee1afc9652d0228a5819da87c6f3b86fe26afe6a68c817070d114946`  
		Last Modified: Tue, 07 Jun 2022 06:09:53 GMT  
		Size: 3.5 MB (3477476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
