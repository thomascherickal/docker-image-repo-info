## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:53f9356992e609911ce2e902299d3ec0ebf860aff4aa489f12b8b44b57077711
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
$ docker pull buildpack-deps@sha256:89525570cc62a18f90b561f94ec9111ecff87157767181293ecb06c475c671b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129826986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10abb968ca71a1bf00261959ee253d8e4c332736ac2ea81a3df52e6f72d5bd22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:44:37 GMT
ADD file:859abf2d579747b132742454ad96e32dc879955afff8af84fab63dc41312a0e0 in / 
# Wed, 20 Apr 2022 04:44:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:00:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 07:00:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:212be0dc3a8ffdc400158a5e3a9812f7413dbb5a86269ff50e41b84b37fdb9f7`  
		Last Modified: Wed, 20 Apr 2022 04:50:51 GMT  
		Size: 56.1 MB (56112566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0603dc0dbc00177fa56a8c1af60fd29d0bf2e8e1e8df8772164b08d8ba1ac`  
		Last Modified: Wed, 20 Apr 2022 07:07:58 GMT  
		Size: 5.2 MB (5209066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da99ea31fc35c2341d30c71a1992c692753c04c61b2e1c25053bc3f9d269992`  
		Last Modified: Wed, 20 Apr 2022 07:07:59 GMT  
		Size: 10.9 MB (10924522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a400dfe0377271d31b8196be8ab40ac2db5aa00dd677d631d372b1df286ddb`  
		Last Modified: Wed, 20 Apr 2022 07:08:18 GMT  
		Size: 57.6 MB (57580832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8439fb8b385f8cc11abcd6183924c2b48f3a94cd6399032750ba3d6967d186db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124495170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dede622cdd74a63b8d99b43833aef742deb88cb75e710c1e5c8476dea3ca5be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:20:15 GMT
ADD file:5cf288f7326d2adfff5d4d3ad0b8951ab86c23ab83cbd1d7799d5c3f7e16a857 in / 
# Wed, 20 Apr 2022 07:20:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:47:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:47:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 12:48:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8db2a46143e157b04953cf05194b0c408afa491a70876185538ed8dca91f9f55`  
		Last Modified: Wed, 20 Apr 2022 07:37:08 GMT  
		Size: 53.5 MB (53518487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341b88f54fc68d22e9e84a8661e65a14684ef134f7f3e5501db09108de37dcea`  
		Last Modified: Wed, 20 Apr 2022 13:07:30 GMT  
		Size: 5.1 MB (5105948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36b40c86c120d43041e78ed7cce077bfa51b33140635f860a17b56fd9349f04`  
		Last Modified: Wed, 20 Apr 2022 13:07:32 GMT  
		Size: 10.6 MB (10597935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445e44e0b7b81da5c386d988323b74e27b2d376a346d93dee764c34c229b7cb8`  
		Last Modified: Wed, 20 Apr 2022 13:08:23 GMT  
		Size: 55.3 MB (55272800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dd942e809a244ec17f986c7b24d421f7046454f05a3477ab4578e9cb3bf1e70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119170493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9825e008287664fe695890dd3c588e5f8760590ce5ee8a6d20d98337bc9565e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:22:06 GMT
ADD file:c6f82841459351fabc9a42dbd56f6622b4374e2c684eb76537d4f31022fe8774 in / 
# Tue, 29 Mar 2022 02:22:07 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:13:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:13:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 20:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20059c5e4ca7052150ded6116965ea89f37bd64493315e1aa29821f6adc82ee1`  
		Last Modified: Tue, 29 Mar 2022 02:38:27 GMT  
		Size: 50.8 MB (50813342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eab1cf1d505662ced1ce7ca793d43715faa8d1006efb38ac9d64a5e87e1feb`  
		Last Modified: Wed, 30 Mar 2022 21:35:47 GMT  
		Size: 5.0 MB (5034266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5291d60208e61bb5100bd38f070ffe9315b62c07b8c223c04ed5c0a722d4ee4`  
		Last Modified: Wed, 30 Mar 2022 21:35:49 GMT  
		Size: 10.2 MB (10244538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c95985634f6e45b9a1cb716fc2e34f25a6f13403cfa0a4d1a09cb9d6670b76`  
		Last Modified: Wed, 30 Mar 2022 21:36:37 GMT  
		Size: 53.1 MB (53078347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fa0a1d0743202d712e076273d5d6e54530a515a9b629b527ee639640aced1d17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128525138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d47665dc88b10e3ec024d39c07c4474e932954e98af456ac2c542b181138f9d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:30:37 GMT
ADD file:21175f4b5f80ba5d755041ff362152a8991b53f89e3c6699275e0c99f6ff6acd in / 
# Wed, 20 Apr 2022 04:30:38 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:47:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:47:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:47:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:414d522b7454847f294a8c61536f57f36cb195df33ab1fce8c838de3d5ae109e`  
		Last Modified: Wed, 20 Apr 2022 04:38:18 GMT  
		Size: 55.1 MB (55063805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc9a9c4b1c386c65ac98874ab622afc88e90b73f7a0e1c692ab412bdd01c571`  
		Last Modified: Wed, 20 Apr 2022 06:56:31 GMT  
		Size: 5.2 MB (5195986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d918141859173a7d14691da560e5afcbb7c353d5694d9541d73f88867578c95`  
		Last Modified: Wed, 20 Apr 2022 06:56:32 GMT  
		Size: 10.7 MB (10691633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541426f7af00f836dff3b2b6976f4053e14eb4fe2fe3a8f804c6b8781c7c3fa0`  
		Last Modified: Wed, 20 Apr 2022 06:56:51 GMT  
		Size: 57.6 MB (57573714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:943ce3ae3c525b37d4092d548129a5c4069582e648d85b6f1cd73fce7aeefcd2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132646725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1922d4df210d4d5cce69ba302f70f95fa3ce71030382cb8708c79dc2b427a41a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:08 GMT
ADD file:92a4df746589380f0ee875ec89574f67fa2f56164bbf20da79eaa902a778eff6 in / 
# Wed, 20 Apr 2022 07:39:09 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:20:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:20:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b42fb3c96c9db2aa67a5b3b033791b735ef01e8c8f15321f44a085532b703190`  
		Last Modified: Wed, 20 Apr 2022 07:47:30 GMT  
		Size: 57.2 MB (57154017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00924a45119800495fe2fa0b6d6aaf354e649da6676746c97c18df9c77e13002`  
		Last Modified: Wed, 20 Apr 2022 10:29:51 GMT  
		Size: 5.3 MB (5340392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faa8d253e5b8d891d6ce9b90e438656a4b5f68ca7b4dfb8f73c36b3da2e9043`  
		Last Modified: Wed, 20 Apr 2022 10:29:53 GMT  
		Size: 11.1 MB (11104264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f2bff506a180a1affdf12a35e0f3c11ba1731569fd21a8a49b19251f503f8a`  
		Last Modified: Wed, 20 Apr 2022 10:30:13 GMT  
		Size: 59.0 MB (59048052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5f7f196fae9058843071d765131fcd30abe3a17f325a3d3107d9b076e2da9401
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126557647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f2298e50be908bcecc4e97dcd0c19a3fcd833e0828095d65a5c8107e4a9b57`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:45:15 GMT
ADD file:8f554d1fa0414c8c5592687851c7ff4646547038f7d464423b75f57ecade0e16 in / 
# Tue, 29 Mar 2022 07:45:20 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:45:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:46:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:48:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:024c5d1fff33205caaf39b2903eafbff594af3ca19d825c46db9f726a37cdcd1`  
		Last Modified: Tue, 29 Mar 2022 07:56:21 GMT  
		Size: 54.5 MB (54453471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1267a248cdd21e2291d70a49d2f9b0a81d371a99832c18a5c27c5cdfcd4ec4`  
		Last Modified: Tue, 29 Mar 2022 09:41:08 GMT  
		Size: 5.2 MB (5222051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240eba6da1031777a8269c912451066c83703897876489a9be1d5150c27d785b`  
		Last Modified: Tue, 29 Mar 2022 09:41:10 GMT  
		Size: 10.7 MB (10672619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9f55cdc16bc7b9ebb3d30b72adac432c7463267759bd2df4d8aef6337988df`  
		Last Modified: Tue, 29 Mar 2022 09:41:58 GMT  
		Size: 56.2 MB (56209506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8bbcefcf3998fd671394d7e4e2317c7862abdb737fa012ba773876583af07acf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139663978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f91cdb83b11679eeb312a70f969f9dbb2037840e9e729dd399e112873679101`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:24:04 GMT
ADD file:a3e83f143a1077db22a0c3474af3e1641c2c20856ea005f45b8cb6abc754cb26 in / 
# Tue, 29 Mar 2022 00:24:08 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 06:10:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 06:11:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 06:12:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:836a00544655c89c89efabf058adfe305cc708f5259ae1a48e4f895cb836a2b2`  
		Last Modified: Tue, 29 Mar 2022 00:37:55 GMT  
		Size: 60.2 MB (60217263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cf9a6305a83e9b7a3d1e30896225843f3509617e9eae396ca2ff8c32153968`  
		Last Modified: Wed, 30 Mar 2022 06:28:38 GMT  
		Size: 5.6 MB (5554821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568b61daaaa9bc8bcd70294105bc93761ba802f89f1ec7a66e7fa6694fd35893`  
		Last Modified: Wed, 30 Mar 2022 06:28:38 GMT  
		Size: 11.7 MB (11703266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55935789c946c332cc704d27439685dd88382de1c7c3382adfba06f00c4aadfe`  
		Last Modified: Wed, 30 Mar 2022 06:29:06 GMT  
		Size: 62.2 MB (62188628 bytes)  
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
$ docker pull buildpack-deps@sha256:f0f7d03377aeb13b3702c16a615167883d858199a9ffe7018ce819100b7e8aff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127234276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008f0528cf59906fe56d1772a3c4fdacbb27d1abc0c68c5318bac1e5678334d3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:42:10 GMT
ADD file:39be572f6c0b3f6f84497807d4bcb370f80b4ac4167f1857002b5571a4dba6b2 in / 
# Wed, 20 Apr 2022 08:42:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:21:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:21:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 11:21:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d9529e5f0bb592a3bb453a841aee9e6a765fede232bccdc538ec2c8b96421d2`  
		Last Modified: Wed, 20 Apr 2022 08:51:05 GMT  
		Size: 54.3 MB (54330969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8df2c317b7e7ca98f001f2d15c613527928de02e7eb3e9f728cd782b7338cf`  
		Last Modified: Wed, 20 Apr 2022 11:29:56 GMT  
		Size: 5.2 MB (5186233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e828f9d86f39827cc0435a54750db181b2f8df2785eca1dddfe35a5536c021f1`  
		Last Modified: Wed, 20 Apr 2022 11:29:56 GMT  
		Size: 10.8 MB (10818188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7992815e0e3b1d2397114927abda25dc906ea8fce59d9acb7a8cbb8c4c2e98`  
		Last Modified: Wed, 20 Apr 2022 11:30:11 GMT  
		Size: 56.9 MB (56898886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
