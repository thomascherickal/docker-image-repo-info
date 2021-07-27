## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:7cd25c1f96bbfc41293624a636e705be39ce2a4e8e9d3d4ea17647dcd7d345aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d86fa220ec910630351b465c36ec06dff76bee05696b129299e2c652fc02770c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81854323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5862355d4afcb1279e2c4f94df12c33a3edf245e67c761982addc0a96aed5f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:41:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b43550a14e1f5842c45eaf5b0043a8aac335974d12b11847980b58fcfd5416`  
		Last Modified: Mon, 26 Jul 2021 22:10:05 GMT  
		Size: 6.6 MB (6644948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e59c30206e4fabc53c96ec7a836fcdc7cdac49cb93fc1b8e376733f4379cfb`  
		Last Modified: Mon, 26 Jul 2021 22:10:04 GMT  
		Size: 3.0 MB (3022291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83c7b2c1eed3a521091d24d714249fb2ee4d8497ba2878141cdd2e4ef3307ef`  
		Last Modified: Mon, 26 Jul 2021 22:10:23 GMT  
		Size: 45.5 MB (45478045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eb9be4475bf74a12bd2dc33ceda28b14add9042751ede89f1fb2a6d9faa22520
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71278028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76e3a6ee7bd29db1e8e162d6139a74479adf24b065995e04ca0ef15da83f92ba`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:14:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef2837cc6a640557235061b89ed9a389330802f062137cb313376de279870b`  
		Last Modified: Tue, 27 Jul 2021 01:40:03 GMT  
		Size: 5.7 MB (5715357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec9e4b1e75d299207a4006fe43a2e34c3fda90619c762ebc07dc792b034642`  
		Last Modified: Tue, 27 Jul 2021 01:40:01 GMT  
		Size: 2.6 MB (2584467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1b636a25e91fe1c88dd15eed3996e0fab60a372c08ebd491408a5eded9d63e`  
		Last Modified: Tue, 27 Jul 2021 01:40:45 GMT  
		Size: 40.7 MB (40671352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8d2e7681306ea27eea801ca12381913a415e70899453fecaa120a3662d140407
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75867846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43eb8abc1a714d61ee7e0df001c8b4f0c448fd76775adcafa140daa5a7f5e7`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:27:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:27:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:27:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb75b79adf2c2db5daeb9e8eafc865ec4b7264bf69d5924cb10268a597758eed`  
		Last Modified: Mon, 26 Jul 2021 22:39:12 GMT  
		Size: 6.1 MB (6085997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d285c9ef2df1931000551273d871814c9eab210544f3926f1187cdcad9e3a3`  
		Last Modified: Mon, 26 Jul 2021 22:39:11 GMT  
		Size: 2.8 MB (2783021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ec9d896f6f86987724a2603cb7fd55032db997c9f79300cf7edef8ffa68919`  
		Last Modified: Mon, 26 Jul 2021 22:39:31 GMT  
		Size: 43.3 MB (43267231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e91841b6197a559975d92e72c7ae799f25280ad3a693c8640369b462433eaeb0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84411720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2f48ee6ff4c478e9996bf6b5efb685723a04c5f9da5b8753072cc154c7527af`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:18:53 GMT
ADD file:45b15f7ce91c2c05cc5e273dee6b36fade4217c3da1d407a6dc8e108f50e2b66 in / 
# Mon, 26 Jul 2021 21:18:53 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:37:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:38:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bc0a67b78038e09ba1732c1a7c63e6c8e924aca7029364acd54d64dd669b151f`  
		Last Modified: Mon, 26 Jul 2021 21:19:48 GMT  
		Size: 27.2 MB (27162925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ac3377a9f0e37ba57c3b58f1e08bc4c546d05fb691aded85bb69e5a08f4048`  
		Last Modified: Mon, 26 Jul 2021 21:48:58 GMT  
		Size: 6.9 MB (6933087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654fa7620a9487b333749b8148fab883c2a84748dfea4659713feb7029e2a4c5`  
		Last Modified: Mon, 26 Jul 2021 21:48:57 GMT  
		Size: 3.3 MB (3252173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1319a834af8832f2159b6fddd4b43bb4e4c65aca6292eced76e342490523446`  
		Last Modified: Mon, 26 Jul 2021 21:49:20 GMT  
		Size: 47.1 MB (47063535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:18d8d370e10a6faa1e2765ce2cf027ddfa6f923e667f65dddad38f75662faa65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94919515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7eb0b44b57ecd5baf3943b3ac62bc88bbb4cf5f8bae752e89e42d92f3423843`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:29:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:30:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 00:35:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e8b2608a7380dbb9682c02133545073ad1fa5bd2baf8ef428031921f0520`  
		Last Modified: Wed, 14 Jul 2021 03:15:06 GMT  
		Size: 7.1 MB (7056284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e159e57607526a57e6cdcdf867e38598e078223ca53c1dee3c5cc254ddcd6e`  
		Last Modified: Wed, 14 Jul 2021 03:15:01 GMT  
		Size: 3.7 MB (3719641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ad8f74299f782ec5a6051b302e0455a1cca5f992fd3f4c5433b96b2d601dba`  
		Last Modified: Wed, 14 Jul 2021 03:16:22 GMT  
		Size: 53.7 MB (53715603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:86b2a03a2bc07a541d53a7ce8defe9cd87340e06c20927d0a0293e2cc151f7bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79692512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b936d8c1f345460daf175e17d73eee9697bd264322183c5dd4b8c6f82ec0b54`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:03 GMT
ADD file:edb1df135699bb6ca591e6493c0df55d2030d8990c3e0a3afa80442036f92e16 in / 
# Mon, 26 Jul 2021 20:55:05 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:39:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:39:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:39:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cb0153f85b121ce88ea3f3bebbb54c31f8547bed022bd201416974cd40c61f59`  
		Last Modified: Mon, 26 Jul 2021 20:56:50 GMT  
		Size: 25.4 MB (25367016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cab3595cecf4b98caf5e79906a75ab2b097f2188f30aa1c7076a0163015ef4b`  
		Last Modified: Mon, 26 Jul 2021 21:47:41 GMT  
		Size: 6.3 MB (6334684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0d32aa2cf3feae7abe26c1dfefcebdd5b24ff1f0db71430b09abe7fff5d017`  
		Last Modified: Mon, 26 Jul 2021 21:47:41 GMT  
		Size: 3.0 MB (2974961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc3c611391cabdfed5dc46bbf421d29284752c25cc449538695bfa4fc865e5c`  
		Last Modified: Mon, 26 Jul 2021 21:47:56 GMT  
		Size: 45.0 MB (45015851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
