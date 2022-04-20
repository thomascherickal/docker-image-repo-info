## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:82b760184b27f1f035713c892a17fd43114a09b1be8ddd7f5a9d3f27ce76a28c
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

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9bb059333b42b6b6fb5e4f22a5cba79e63fb900c2fd0acdf2053c150115f95e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124044920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f03d664de27b2ae88e5af86f286eb50c16e07672da0c733db19b9733b01dbb9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:53:53 GMT
ADD file:8fcd736cc488ae6bc3f8a0a57f5454dbd34b0c05fd62d2bf748eeb34723c2a85 in / 
# Tue, 29 Mar 2022 00:53:53 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:53:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07dd120b73b0ec25351ce0c0743306437c1d81e0ee7e06f053f28a0e58bfa81f`  
		Last Modified: Tue, 29 Mar 2022 01:09:52 GMT  
		Size: 53.2 MB (53206463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182e180f96ffc4d0dea65f46ebf08c1601dba09f8a2bb20ff2f15148ff227cfc`  
		Last Modified: Tue, 29 Mar 2022 08:11:41 GMT  
		Size: 5.2 MB (5164114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3369a2a9d3d9efecc9720a25d251260ac8afb4a7a974b188960c5a1759c27c2a`  
		Last Modified: Tue, 29 Mar 2022 08:11:43 GMT  
		Size: 10.6 MB (10597701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc501bba1675670306129a4d527e61027cd5077d145db1dbda301297e9f32004`  
		Last Modified: Tue, 29 Mar 2022 08:12:34 GMT  
		Size: 55.1 MB (55076642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

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

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

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

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:adae09ebc335c11ebcdf5e6eea0972a393019b3ea5a07c01c1498a1680cada09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132216228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7509be880a8b7cf31d596698ced4c3183a024074527d024f18d4e0d8522370fc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:25 GMT
ADD file:a09b15a232ef12356f8a381e48ebbc75da16b46600e0cc9849189196595b48b3 in / 
# Tue, 29 Mar 2022 00:43:26 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:00:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:00:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 18:00:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0847c00642d4fc3cd086952d88bb1c62b35fc1592abb8bb98b5f2580cbdf5cc5`  
		Last Modified: Tue, 29 Mar 2022 00:51:53 GMT  
		Size: 56.8 MB (56838514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358597cf26cb0d69578f67ae8478edc056e17062702b8e9b5223d5ef224bce7`  
		Last Modified: Tue, 29 Mar 2022 18:17:32 GMT  
		Size: 5.4 MB (5399988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229c59efca77e15f2eebc343a63ccaff506b30dec30f8514f410554d9016a9db`  
		Last Modified: Tue, 29 Mar 2022 18:17:33 GMT  
		Size: 11.1 MB (11104016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c14fb78209a987db23cdb8ca3da7ea675992fd648530b5b3cf73a82bc0598e`  
		Last Modified: Tue, 29 Mar 2022 18:17:53 GMT  
		Size: 58.9 MB (58873710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

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

### `buildpack-deps:unstable-scm` - linux; ppc64le

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

### `buildpack-deps:unstable-scm` - linux; riscv64

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

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ab4e6faf514c30d680823bcd44ba55ee346331c520e518338c75516dd4479bd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126921779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba4b29813f22cfa4231622481c53d40afce8c4cfe14c9ba4d5d0231566f7816`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:53:06 GMT
ADD file:5143c5815a4282433726df7dd89926b3676994be1b8575d259b8fb48d6a6a4de in / 
# Tue, 29 Mar 2022 00:53:09 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:28:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:28:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 02:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c86b61bc0bc235576e3d7696ce7a1c21762146f539dc6eda8173ad30b9a4ad20`  
		Last Modified: Tue, 29 Mar 2022 01:16:39 GMT  
		Size: 54.1 MB (54056452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcff4b07483f3bf89081280922e0b152bf4d0bd3c9886eca04d4701cdfdc8bd1`  
		Last Modified: Wed, 30 Mar 2022 02:35:19 GMT  
		Size: 5.3 MB (5255620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34095a4004eb76305dc89b1fe0dd2923e12bd88528d9b779fd1ba62c9ccf1ed7`  
		Last Modified: Wed, 30 Mar 2022 02:35:19 GMT  
		Size: 10.8 MB (10818241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1369c129afe9ff16634f66b8ce0ef29c35ecd9d7bd06e6096ad4ad323968e9f3`  
		Last Modified: Wed, 30 Mar 2022 02:35:33 GMT  
		Size: 56.8 MB (56791466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
