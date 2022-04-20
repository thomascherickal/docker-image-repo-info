## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:e44f014e1871e8742bf0714a57cad0790873cac5350722085eae5d9aeba38537
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

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fbc80cda6f350aed47ac3540388b4dce8bfb11cebb27c525f8b1203bb7bfb8ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68290594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a58de45849f73ccba1d8170cee14f5df0f5176341eb3f53d33e5771ba040578`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:59:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdd409f4b2bf3771fac1cbc2df46d1cbb4b800b154cfc33e8e0cd23e67ab3e0`  
		Last Modified: Wed, 20 Apr 2022 07:06:56 GMT  
		Size: 7.9 MB (7856378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3069e6cecf9d5e43ace0a925b53849b2fd189ef41883d45d8f2e12213c2c06`  
		Last Modified: Wed, 20 Apr 2022 07:06:56 GMT  
		Size: 10.0 MB (9997231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d345d0e6bbcd39917820aef59466b6004ad627d6343e31e9e9713cd9ff04c80a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65246421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ac1fa34e52ac613189712d9bd8f7222e6efb3adc980da31741c8530a562bd4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:04 GMT
ADD file:e7d31ee8f990df96d5922feb35173a364a0832e8fce2d32fd4e703aa3b66e1b2 in / 
# Tue, 29 Mar 2022 00:51:05 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:46:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:47:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0bbc2517bf9c8d842997ba8f85b59bfd92c5bb6bba79c39047eecda859dcae27`  
		Last Modified: Tue, 29 Mar 2022 01:06:08 GMT  
		Size: 48.2 MB (48158294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1b4a5e78fec7573050b1b9220718c42ec377971effed53f70015af0614fe3d`  
		Last Modified: Tue, 29 Mar 2022 08:08:45 GMT  
		Size: 7.4 MB (7400493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4f39bb570fd924ca89ef560a7dcf08a5b1bdb060fffc39839196ea306860e0`  
		Last Modified: Tue, 29 Mar 2022 08:08:45 GMT  
		Size: 9.7 MB (9687634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7c070c3a35c160408e5ddd669c5a0cd0b6cfa101d99559143663e2f718a3252f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62403380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249bb5194f8b63d20ee9ecb406426ec8f154095cbf8b095ac50eb6dc0176d6eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:04 GMT
ADD file:60a690e302d164c569e6f3fc29adb6686618bb728249405f90960835525b0599 in / 
# Tue, 29 Mar 2022 02:19:06 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:09:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:10:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0cc72482f2e040b686190f2967010d45947924353440070552a298b9f9f81b19`  
		Last Modified: Tue, 29 Mar 2022 02:34:54 GMT  
		Size: 45.9 MB (45914531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ee42f432eca8b10b5cc28da57027f157052392220ed81ab477a06ce1771abe`  
		Last Modified: Wed, 30 Mar 2022 21:33:01 GMT  
		Size: 7.1 MB (7144979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bdeb2a3bd0d310e035553bfd8dca244c71e5c1d7fa33c8e1f19d5912e0be7e`  
		Last Modified: Wed, 30 Mar 2022 21:33:02 GMT  
		Size: 9.3 MB (9343870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b60aaa17bc8dfd23b53ab35ffe383a0ae27f08334d94118361c7ca6713ecb5bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66714795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950688e26dea003683c2536e85d7087f6c6fff77fdc83c71d5d2aa74b4ed39d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:22 GMT
ADD file:5286ff5db23c42ac6a437e8f2f9ef01b6ee6e523d7866c752428d54f177c7108 in / 
# Wed, 20 Apr 2022 04:29:22 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:45:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:45:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b9f330b3a7e234282d632d95bd19a655cf0e06c1a76a51d0f73b9581be8f851b`  
		Last Modified: Wed, 20 Apr 2022 04:36:12 GMT  
		Size: 49.2 MB (49227738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80651adb7e52d8ecd27d43b9e69ada9ca277071ea09607121d0076de36480b`  
		Last Modified: Wed, 20 Apr 2022 06:55:25 GMT  
		Size: 7.7 MB (7719745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b38ee622cbfb492ebc3bc598771624fba7ef1830b4e0f9737f2bbf4b6ec0ea`  
		Last Modified: Wed, 20 Apr 2022 06:55:26 GMT  
		Size: 9.8 MB (9767312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a953960e8bf760e5897ff002086c039ad360b8b0195a99b467f9096c1f69a788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69340157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8ca179b462131348aaa1d4369d014f2d81bac00e658d22bfb600cf4df8d2407`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:47 GMT
ADD file:f66ba5e7b2801d19041661506f244a3bb89fc613e2e27891bdba3183bd6ee097 in / 
# Wed, 20 Apr 2022 07:37:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:17:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:18:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e8f333ddc9f58dd9e74b1f250e3812ba3942ef13abee1d6b4e3d3131a7e29ff`  
		Last Modified: Wed, 20 Apr 2022 07:45:17 GMT  
		Size: 51.2 MB (51195868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4353b7b00b407b29561abe4d0fffed162775a58e3c48ee2edf64cbb21cfcb11`  
		Last Modified: Wed, 20 Apr 2022 10:28:45 GMT  
		Size: 8.0 MB (8022285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f90dfd06367deaf8c4c4f802c2dfb9a36dbfb3d208f4972a8c79b0892b07832`  
		Last Modified: Wed, 20 Apr 2022 10:28:45 GMT  
		Size: 10.1 MB (10122004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:00c26d0e540adb79c57370e8350929192083dddd6f30caf3f6c8e56775ae6ff7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66152937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a46cf9ac853b8c13da1a63df8a38527f1ebb60174f920af3601389504cb3b57`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:43:01 GMT
ADD file:c86010b52f782f910842586e6abc81e64c7a659d001b89799314a59f4fb96573 in / 
# Tue, 29 Mar 2022 07:43:06 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:36:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8e0bee9c4b9257c0ad7469830be5e890536feef4e8ffe6c2613b7e8be7e060f6`  
		Last Modified: Tue, 29 Mar 2022 07:53:41 GMT  
		Size: 49.1 MB (49079891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc690a0cd1092524bdd12063c730cdf1df3dfa2f8c5920231d8477654c04b854`  
		Last Modified: Tue, 29 Mar 2022 09:38:05 GMT  
		Size: 7.3 MB (7272773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe0e6a034874e5b70e892d14e911e5aaa7f314b7588616996be6ff22190b1a`  
		Last Modified: Tue, 29 Mar 2022 09:38:06 GMT  
		Size: 9.8 MB (9800273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a82ed0848001a5ce880f824333fb3412dce09bcdfaff66c9e47681e2d8c28d3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73204220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c16db849f7963b1ee9a8f9c57d7bbef15f7a77820de34375f1651d373ae6e93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:25 GMT
ADD file:a600709d679cffd058d04ba0eb0765cc870766fd5de083ada0eeccfd7afc21f8 in / 
# Tue, 29 Mar 2022 00:22:30 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:59:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:59:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:eb53bdc4c2c6ececbd424b1c643b9877934a5297a5d2db0eca1a175d7a21d32e`  
		Last Modified: Tue, 29 Mar 2022 00:33:53 GMT  
		Size: 54.2 MB (54183100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596f9130bbf698f182cdd8f8965c6d1fb059aff38e309f7dd44db12967d4ab7a`  
		Last Modified: Wed, 30 Mar 2022 06:27:07 GMT  
		Size: 8.3 MB (8293334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf74211bc82c5c0431e1ac0b76c006093e829ef420568923567cb2d6bf07a69`  
		Last Modified: Wed, 30 Mar 2022 06:27:07 GMT  
		Size: 10.7 MB (10727786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8f8bd2a1d7a7f6e9e17b89e2f922d11a95aadc75aad67f61f0fb3deb5a8bafd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66314325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a162a38df2214484b29d79de0b23c173655cc21e12682f750893f6036670456d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:09 GMT
ADD file:784894d175880656ac82b485076fb224bde46d379dd634720acf7acd5eee9365 in / 
# Tue, 29 Mar 2022 00:52:11 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:26:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:26:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e3cc532be5698da8ac6589c11495b960fec83fd52aa82617e3218678ff4546d1`  
		Last Modified: Tue, 29 Mar 2022 01:07:20 GMT  
		Size: 49.0 MB (49007755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af67f5247c69c4ea0f2abac4f0d15b87aba276b2900c5741a7c88233a7be56d`  
		Last Modified: Wed, 30 Mar 2022 02:34:32 GMT  
		Size: 7.4 MB (7423528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1254cde0440f5ac2b199af47f310c376960961694f11b68a43cfc6a91c63ff`  
		Last Modified: Wed, 30 Mar 2022 02:34:32 GMT  
		Size: 9.9 MB (9883042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
