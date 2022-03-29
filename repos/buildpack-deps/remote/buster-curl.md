## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:a090bcc684317f9d6fa33ef618b50aed1c65dece210990f3461df16deae8fdf6
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

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8b4870601c99e26bdb0e9d6cba7c9ef7a1efec911cdfc1f59ca1d087e10afc84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68291508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5632c1efb61eab5d42fec11ade19c955f613597e5433191c4af806f2ee861243`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:28 GMT
ADD file:8c5e9f12fd3b6e830ec0ee1800d8e9dcebf217896148f2dc72c010c8a88d9b8f in / 
# Tue, 29 Mar 2022 00:22:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:31:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b281ebec60d2630a225601bd58a4681375a31b7316263b64d3b149f49694c3fe`  
		Last Modified: Tue, 29 Mar 2022 00:27:37 GMT  
		Size: 50.4 MB (50437915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dae484504b039004d1f23b1777be24e9e8d0f126ee1f38b97544d6343fb9fa`  
		Last Modified: Tue, 29 Mar 2022 17:39:22 GMT  
		Size: 7.9 MB (7856401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21739e3ef21a7c9983fdfc82d5a3837c633779965fb0b2cd7b746ec9c260664b`  
		Last Modified: Tue, 29 Mar 2022 17:39:22 GMT  
		Size: 10.0 MB (9997192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v5

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

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6f425e165bb91ab3b64b08bb180c8d1cd2f57c161f2a988cfe8511734560464a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62387581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3ee701a8a316cf75747a30d4b9509d087aea34944b7a8c9caef80618a9e5d8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:32 GMT
ADD file:7fe62421fc35de4e6311d22de22ded33c729d98a51fa41d57e04c76ec092827a in / 
# Thu, 17 Mar 2022 09:31:33 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 02:56:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:56:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f82e094db40ddc4d9b2e16ec4c7f28c689bdd532358e18ab566e90aa5975838c`  
		Last Modified: Thu, 17 Mar 2022 09:47:22 GMT  
		Size: 45.9 MB (45918162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6141a0e962d9abc8740d150bc5bf7f5a58f74cc0e97601134c7ceccc5dc31eb3`  
		Last Modified: Sat, 19 Mar 2022 03:32:03 GMT  
		Size: 7.1 MB (7125521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529c02d4e740677c379f14554a5eea0184ff342fd3986da4914383e499ccb1e`  
		Last Modified: Sat, 19 Mar 2022 03:32:04 GMT  
		Size: 9.3 MB (9343898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:13b805388986d203beb8a143f8ad4bfc4102e1cc40a7992098fa845ccac9a727
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66685545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96384cb262ca4b16a0bb18a01add8bfcbb6e008497af8df0e6276c3ac95ac47c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8e6c357ff29435e2a16bb9e6a5077e0e113e55587d9ecece7969c347f88120f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69350713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dc526298aa96723eeb244b4ab53eeef4e521e55b2cde6f6af11e3c7328767e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:12 GMT
ADD file:fb2c1bf394c39b5bf948ceaa00317518326bd846b3f6802dc39cfb7fcf404c69 in / 
# Tue, 29 Mar 2022 00:42:13 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:58:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:58:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b86fabf064e35595b9c8543deb0dba50a95e438387a9877ebfe189bbfce3c87b`  
		Last Modified: Tue, 29 Mar 2022 00:49:34 GMT  
		Size: 51.2 MB (51206670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fecf9ef7e2149c926eaf909af17e48d32080f3777447e28017d8277168ef61`  
		Last Modified: Tue, 29 Mar 2022 18:16:16 GMT  
		Size: 8.0 MB (8022197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ba7e132575662e21e001c19449819145d8c04740ee029d58abb3883fa71010`  
		Last Modified: Tue, 29 Mar 2022 18:16:17 GMT  
		Size: 10.1 MB (10121846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; mips64le

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

### `buildpack-deps:buster-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1263b525ab0a0323bfc85e714a22403bebdd02ece0f02e115a36165e598337d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73185192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d59910509cdee28de690acbae1c6de00279fc809fc126fe6e8f801a0202c6a3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 11:18:17 GMT
ADD file:f75a960e2412d5d93ea52573154078e69481bda1da84f66aac3871c0c0776bfd in / 
# Thu, 17 Mar 2022 11:18:29 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 05:48:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 05:49:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c525619180c8f2ab5210413380ee35a9d0855c7e877e0ebe8841a1724e9605fd`  
		Last Modified: Thu, 17 Mar 2022 11:28:49 GMT  
		Size: 54.2 MB (54183837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab80fef29bfe486fc89cd31900757a3db86e74b037ab36d6d675a9d3ce9e750`  
		Last Modified: Sat, 19 Mar 2022 06:42:35 GMT  
		Size: 8.3 MB (8273595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60d3aaebf7006e51596f47c9c245b72f01999ee68dbd0071b1903bfd578386`  
		Last Modified: Sat, 19 Mar 2022 06:42:34 GMT  
		Size: 10.7 MB (10727760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a806c4c12568931cb2ed0fbd0489d31a4882a4d805be9755bf4af40368869cc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66290297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a04780d8387099d759848dfea68450567904614e65ace0917a2fa30e16ce4d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:11 GMT
ADD file:6505b8e134084dbb9f879838b24cf47cd265cfdc5952f50ba2ddc63ff4553145 in / 
# Thu, 17 Mar 2022 03:07:14 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:22:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1e9fa32475c4074341da88d0325d6e125bf7587795cba4bef553a90bf7472c7b`  
		Last Modified: Thu, 17 Mar 2022 03:13:01 GMT  
		Size: 49.0 MB (49005525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dfc7a2d5d979460a379f74fd1adf756566aaaf27b9ad22b518b7b0b13b7b2a`  
		Last Modified: Thu, 17 Mar 2022 18:29:59 GMT  
		Size: 7.4 MB (7401708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1517a8cbcd9e9cd84fd94cb3e7e7a02def9f47cf27b751461484d31f85725361`  
		Last Modified: Thu, 17 Mar 2022 18:29:59 GMT  
		Size: 9.9 MB (9883064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
