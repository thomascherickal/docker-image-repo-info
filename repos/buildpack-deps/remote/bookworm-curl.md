## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:9f8c8a5999313d34a4a92a504e9cafebb0e8b3d13501bff984b6eb64e3c06d4a
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
$ docker pull buildpack-deps@sha256:65f4152e56d007d77c7d77e60f052056273d3a9ecd93ec0ee27f03e9d06c15a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73642716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4264bd0b8285ea524f31b2355c6cd723c750a6c269a38987e6a7776185b1666`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4c3fea69e1e4777e0477d2bd05fe0a928dac89285b2485e281c89d33f1116888
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71612761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:159dda42248d4464a45912c2782dec3cd5c2cf073da7e38e5ab9a9ac80cde99a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:48:31 GMT
ADD file:2f3df348b6a9200fcbcfe13a10334cef72dca5f19d7ed73055f7a03ff08122f7 in / 
# Tue, 04 Oct 2022 23:48:31 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:12:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:12:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2843f1fd91937d710e0d158046e9c23fe034f11c8c934a478f443b561be758dc`  
		Last Modified: Tue, 04 Oct 2022 23:52:36 GMT  
		Size: 51.8 MB (51838659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cbaeabf686852f0109b0402554bbb882e0b7f95b9befb62dcb2c9cf5334b69`  
		Last Modified: Wed, 05 Oct 2022 00:22:23 GMT  
		Size: 8.7 MB (8744107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b61654d50a40ae8ba57e261eb049904e5e6879f2e9421bb37a8653997b3e6`  
		Last Modified: Wed, 05 Oct 2022 00:22:23 GMT  
		Size: 11.0 MB (11029995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5b0dee0e2cc0e1938cf13bff64e7e8012209764899a65e170b1d0ebc91e645e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68750987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d654a5ab6c7cd35f5bd3a5856e37d1f2b004dd7fd02791250fb62401d704090`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1481632890c7a3ff9c1451626fec55caae7629692e9bdd524847cd9761439cc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73242713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c6b892888321feaf66863a61297f525763ba073853acb3ddda2197f0c5ee3e1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:00 GMT
ADD file:269c8bec4871d84b9133706a2f391209619d53c0bfa56121c740757cf5798fcb in / 
# Tue, 04 Oct 2022 23:44:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:21:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2debf9e7f23054c81a936da9b01c5db9f72a55d4810f7bf0e5641bd1748d90b7`  
		Last Modified: Tue, 04 Oct 2022 23:49:11 GMT  
		Size: 53.0 MB (52980389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a790615211c3ee762ced64a5b81859f93d76062f4cf9c83d396fb13c24f7cf`  
		Last Modified: Wed, 05 Oct 2022 00:36:13 GMT  
		Size: 9.1 MB (9128105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70f6dfe035ba217dd9a40e630bb3cae03e8d9cef649641a8a502495edf00c0`  
		Last Modified: Wed, 05 Oct 2022 00:36:13 GMT  
		Size: 11.1 MB (11134219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:167dce0d41220877a7d69d1e1e4402a1f7db01d68c2ede73609723628b0d8d40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73649206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e11ce92eb7a28e68b38ee4db9094ad80ebf756d2c10f5310aacf4d6fe927bfc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:21:54 GMT
ADD file:f47fc1d53965bb08e38b482e78bd79e3cbeecc53e586ffd88bff0e6fed0a1f3c in / 
# Tue, 25 Oct 2022 02:21:55 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11f88873ba86e184f57ba78457d36c4f22e16eaffb9c293964adc7905e18bfe5`  
		Last Modified: Tue, 25 Oct 2022 02:27:09 GMT  
		Size: 52.2 MB (52224672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683bf09527f61248ec1a0fa70be7388069c28d961ae31bd3a05c43ae41192a7a`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 9.3 MB (9330348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823ddfa7a0daf2e9e0c4b6ce038b2e2cce83bde4ba9aef56fb6911d8241ca03d`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 12.1 MB (12094186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:493af583c74bf77e0b891e256e7da2871572e0ac49991ed4bd9ffed3bc97e620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72758866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:478aeba09b867d6194866aa4f12b4d9bfb445ad80db4cd1a7f24338c467bc945`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5ccbecabed537e9c487c2dc7ec503351ba0cb52a24238ea701d2f4e0307a0104
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.1 MB (79138638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d590241e6109dd3cf4991606afc14594fa1c6acf47ede90f6703f6b7948ca8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:16:56 GMT
ADD file:22dddefde9f3e8eff6049751a459a3c4fdade46622016ce6269b630157170962 in / 
# Tue, 04 Oct 2022 23:16:59 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:47:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Oct 2022 23:47:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8fd653dd210d0ff49ceb9b32e662a564ab01445265e165edd4f963c3953f5b33`  
		Last Modified: Tue, 04 Oct 2022 23:22:42 GMT  
		Size: 57.1 MB (57111564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f7f38b022f1a84d71f8e4124fe0133ced1b702ee627bff0eb3e756558fbdd`  
		Last Modified: Wed, 05 Oct 2022 00:02:33 GMT  
		Size: 9.9 MB (9883282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79064b2f900a5a0fc53fac8232b1268f1f2e3496cc5722826e03a2b768366be9`  
		Last Modified: Wed, 05 Oct 2022 00:02:33 GMT  
		Size: 12.1 MB (12143792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:894b1261a23e6de74babe1ee3f40ba9e50b5c66394124baddfddd8c053c67ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70091131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d41791c8becaef1121c6430e271e2135e1dc7887ebe7a1da86fdacbd5a8eaa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50715b09b75ed5a3b59f5532be8529ac130746e899c823894a3ee91fc976a5ed`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 8.8 MB (8785586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb8ed5a6b2d134cb7b866721196b0adaa54ab94d27c13c65773f16fffc143d`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 11.7 MB (11727044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
