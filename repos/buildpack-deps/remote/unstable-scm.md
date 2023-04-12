## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:edeb47aac306028e88b31af5cfbb056fa15167daaf42c90a1a57b9a12dd85f4f
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

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d9f6278d7e0c871b5bcdc327298a29c7c00a8a0504891c4ad2631c374b75a01c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134049910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd617366d1cce33570b6dcf04f7eac2404f89e0bece798cb7e973cbd704f667`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:54:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:54:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486f0b6179599c75a087e6850c42ef248d973e29a6898ed99c9bccdae08d2cd2`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 9.1 MB (9082764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f184ca8dda7ed83dd9d21d6c880d4e15976f35814156a0a67df81423067f4b8`  
		Last Modified: Wed, 12 Apr 2023 07:59:24 GMT  
		Size: 11.4 MB (11422423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76159e5040abc54c8e269f5e87ba68551c98fa9a6a06c9d7af5eae5f9f3ee57b`  
		Last Modified: Wed, 12 Apr 2023 07:59:41 GMT  
		Size: 64.3 MB (64257071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c0b4a3eae58bd274c266cb60478e79df6446cb058ebcb7beec816064f9c69b75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129365563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b15a5f5bf525f6d5ed1af6bc9d3b44768864d1199c3f26e961d670e918851d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:48 GMT
ADD file:b02c911309a1b69d235b76dab369d523653c62374b0173ee9f1b65017607f9d6 in / 
# Wed, 12 Apr 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:18:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:18:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8699c4859220eb7e4f2a5ae13e4dd5f9143cb7144e2a02a3eb381a79416524bf`  
		Last Modified: Wed, 12 Apr 2023 00:51:27 GMT  
		Size: 48.1 MB (48109671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b565bf44c40ab65f5193c4fbfd752809f50e95e2c4b2397728f42419979d7c`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 8.5 MB (8522810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8db076a21199a98e758a14876a91c9a890bb606e6d9d483862bcb73bc5cfbb`  
		Last Modified: Wed, 12 Apr 2023 01:22:25 GMT  
		Size: 11.1 MB (11065853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466720607b58ed4036916fa9d7cb2e82a3ca95f0e5ec8e2ef908744cd3e409ec`  
		Last Modified: Wed, 12 Apr 2023 01:22:44 GMT  
		Size: 61.7 MB (61667229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4625cae1cb86a704920cb5e233396ab0915f8f8aea6c2991bf83dc37494e5707
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124124089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a34df020edfcb54003832698a6fd1b0d2df01b8d86feaa47193d84801d022ab7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:33 GMT
ADD file:f8bcd71f10e7adad706b3a1685fd5c4844e3ebde65bdf9a7c004d7b9dd3520d7 in / 
# Wed, 12 Apr 2023 00:00:34 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:40:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:40:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 09:40:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b0aac501774f41dc4e46815077e011ed06b86d9469c6ca28755965123669423`  
		Last Modified: Wed, 12 Apr 2023 00:04:46 GMT  
		Size: 45.9 MB (45890234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78f03ccdd59b1aad6c28d38c86bc934c8e0a1da27d7a0be742b455933d23138`  
		Last Modified: Wed, 12 Apr 2023 09:47:20 GMT  
		Size: 8.2 MB (8168595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da6afe7624e90c309b1a605bad2994526027d5e48a341ffc3ea92eb706041f2`  
		Last Modified: Wed, 12 Apr 2023 09:47:20 GMT  
		Size: 10.7 MB (10690111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59c0245364868d7a1a6302c947f5a93b4058f6e740cfb6fdb6e5bb49709f683`  
		Last Modified: Wed, 12 Apr 2023 09:47:40 GMT  
		Size: 59.4 MB (59375149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:909145f5f8b9a67acd7be2b62e379fe6c15950dee01727de50e4cc961c962502
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133786279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c7d9c27ae042d56e7ca69c21a7a5a690294d166c8196d78574264d9160d8957`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:10:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d9e5d2b2df062d16ffea4a022a4c09ce904fb96ec3fa4712a1d936593ae2a`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 8.9 MB (8915031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2b1a4cab3b4ac2bb4a7e9aaaa60ce806e3c49a8726f7baf5a10ba5e0e89fb`  
		Last Modified: Wed, 12 Apr 2023 01:15:01 GMT  
		Size: 11.4 MB (11389544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff14914c0381e1889d1db49b1b39da80ae3a347cf1af048e2ae0eb42aec87a12`  
		Last Modified: Wed, 12 Apr 2023 01:15:17 GMT  
		Size: 64.2 MB (64154048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8e5134589fb0e6d388a1a4741142104956636747431cf809398cd58520b6da78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137529120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acc693ca7c37b5ced8d79a021265f81c4cecbc277909bb33bb103fd1302a0b37`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:11:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145bb18c860aae65312434f79bce9d784a4824ef455202efca0f687a388037fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 9.3 MB (9263774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063c41d1dff24f54b6a7d8edde21610fe37e02b35ed369be0ccf9f64cdc43fe`  
		Last Modified: Wed, 12 Apr 2023 01:17:27 GMT  
		Size: 11.8 MB (11827096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3196dd70f259df7354dba37d732f79f68e602883ec8838b2cfcd0515de5c5c`  
		Last Modified: Wed, 12 Apr 2023 01:17:49 GMT  
		Size: 66.1 MB (66127351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1fe2cb894be2bc55a95b04e66763ccec91305b7c7ac438bca7d21d751c7809b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (132001554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e553975cc4545e2dfa4c801fc4f1bfe90378add106afcf9e70883c34024f725c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:24:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3768b306fba92d6a836552b3ee3a1bb755cd0f7d6618ca028d0643fde06553`  
		Last Modified: Thu, 23 Mar 2023 07:37:53 GMT  
		Size: 63.1 MB (63099163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8135b2f23a71e776729d178ad2c044b029e434a6d8851c6db2bcf9c99af46c83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144882078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1217c66cbb148d338fc6383d0543b5e72c22f88e67d1ad1e01886b46dfed4a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:41 GMT
ADD file:8700846eefa6ef0670106ef8055671479d597d057ee34d1d248dbefa5977753b in / 
# Wed, 12 Apr 2023 00:08:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:37:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:37:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 09:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c14c235d79599f644d6f952e975871669fe8a00e0434e5d26966f11cfb3820b`  
		Last Modified: Wed, 12 Apr 2023 00:13:39 GMT  
		Size: 53.3 MB (53291710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140d550f01a3ea4465718eae23deed53e8c34f53813fb05c7fbbd6718d137b67`  
		Last Modified: Wed, 12 Apr 2023 09:46:52 GMT  
		Size: 9.7 MB (9663547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450886794424f907ac99ffb3d1748b6d36f1ae455fbb553503d88898905d6d36`  
		Last Modified: Wed, 12 Apr 2023 09:46:52 GMT  
		Size: 12.2 MB (12184648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf2504e8cddf5044ea9695b547b876a5177d803d452f5e4e0d8050845be707d`  
		Last Modified: Wed, 12 Apr 2023 09:47:19 GMT  
		Size: 69.7 MB (69742173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:bcd300a4e07d706f2fd9f306c4c32864622137e94ae3c3c4670ea905ee0beff3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124147555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:397d717b57a8049a3da1ad949d9ed38c1e6d2518bf8f6c629c18545c03f04445`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:05 GMT
ADD file:b8c0cf42f791d92283c2c47cf2ed446fb98a7cde685c9b923c89cadb86ddad31 in / 
# Wed, 12 Apr 2023 00:09:07 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:35:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6178d7c3b8603b1579d72ad9f5bda8fd22627feccccd498dad946eddfe96d27a`  
		Last Modified: Wed, 12 Apr 2023 00:12:25 GMT  
		Size: 45.5 MB (45494949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd056fe810f7c94134b5c26af6939949c18bfa4868dbc9f81ea8d7a25a0daf4c`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 8.1 MB (8117374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f8d5394c046224d62d5170fd151d4339e0f5131b1503bf3eafecefe1ec7a10`  
		Last Modified: Wed, 12 Apr 2023 00:44:01 GMT  
		Size: 10.8 MB (10794055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0c6cc5fb9f28304c05335b3e21ed5e3cce359b94731f04cc903938689ebc19`  
		Last Modified: Wed, 12 Apr 2023 00:45:23 GMT  
		Size: 59.7 MB (59741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ab7bb732a3d488865f2b887c55fbefc2e0041d528429e377f1f5ee84b43bda25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130927162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dba9e0d63f399d18f4d3f0cd3f58b4eee0e1d16c71d855c9f9b0bd4e250d67b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:19 GMT
ADD file:0593fbca11f3d4a9b2b916ee99bb70651af04ea1275262f12e9b0e5c07e81f0e in / 
# Wed, 12 Apr 2023 00:01:29 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:28:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:28:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:28:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1844a6b5cc32e25703d3a6ac2115866157b1f856d7463d0dca8443fea51061f1`  
		Last Modified: Wed, 12 Apr 2023 00:05:31 GMT  
		Size: 47.7 MB (47665068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f306dc6c45f3e2637390b46a2dce7fb061bb8be6ae7c72c47bba97d84b99d256`  
		Last Modified: Wed, 12 Apr 2023 00:33:37 GMT  
		Size: 8.7 MB (8713548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676682574fe22f1cac8016a4f36ad54898c4313e0609a7e88e75e035e32444b`  
		Last Modified: Wed, 12 Apr 2023 00:33:36 GMT  
		Size: 11.3 MB (11288124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f9748f029581dd4821ad6e7d4da7ab4a31600128a2411dda2639c9b92fe58`  
		Last Modified: Wed, 12 Apr 2023 00:33:51 GMT  
		Size: 63.3 MB (63260422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
