## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:c097b5f3a34a8dd73d006a81a3ca3d839ad1830c402f14cfa3639795945d6679
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4e8c5a0c7e8b43250bcb142ce3c50bc1042df54800ae8621f268e47ddc153435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125502551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b100c95ffb741a530d138581a453d9f8be7d771e19aa1122d331f1bf0bad0f9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:18 GMT
ADD file:ec1a9a704ae13b142c48069368561119760ccdf3d65d854c426d0dc9c39e60fb in / 
# Fri, 11 Dec 2020 02:05:18 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 20:36:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:36:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 20:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4991c356405721fc787980835bdbf5c529ae12379346a771feb34407c522bd6`  
		Last Modified: Fri, 11 Dec 2020 02:11:29 GMT  
		Size: 53.1 MB (53113553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5372ff68e6e3cd35af447e668d2d3891b5f142a066b5e280cdd15aa03c1c18`  
		Last Modified: Fri, 11 Dec 2020 20:43:51 GMT  
		Size: 7.9 MB (7891296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b568ce8dd7467eecd5668427a68142d78e1b88e8184b46728d118f461256af`  
		Last Modified: Fri, 11 Dec 2020 20:43:51 GMT  
		Size: 10.6 MB (10648130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db7df191a4bbfd3f5a833d696793518a985aef224bd5bb5d80bdc93a6ec827d`  
		Last Modified: Fri, 11 Dec 2020 20:44:09 GMT  
		Size: 53.8 MB (53849572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0462028ebf10d38b3388fd9381c19e250b3c25a1b6bdb22484d2edb26b95de7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120382027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b7eed0d7945ee312a737d7be17851c7cb8ed0bcda945e11ec98e39904c1da`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:8b9117df3f1a986438250b725bc8ec117cf1caba2e6953cf9a870edbcda4c565 in / 
# Fri, 11 Dec 2020 02:03:10 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 01:48:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 01:49:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 01:50:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69233e69b29a579de45732361ee762ae02ccbe96b0f2a09fc2a48a802a25b265`  
		Last Modified: Fri, 11 Dec 2020 02:13:31 GMT  
		Size: 51.1 MB (51053259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f37df2f9cd5b84770356fa5f939540352df527e8614387e2efb5526fb6ba3a`  
		Last Modified: Thu, 17 Dec 2020 02:10:26 GMT  
		Size: 7.5 MB (7461139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b0c8aa368faca2325c1ba58e6f5cab5bd150dfbee94b95963c35d62581f86b`  
		Last Modified: Thu, 17 Dec 2020 02:10:27 GMT  
		Size: 10.3 MB (10335182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212eef771074abcec8b78a98ac45bbf906c1c19db951d76d98bc559350707cab`  
		Last Modified: Thu, 17 Dec 2020 02:11:17 GMT  
		Size: 51.5 MB (51532447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:44589069ba939c189a874f3cab5e439e054db1a833760fca6d86daf781d3487c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115496334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc556a61e5d2304892305c9073b59aec2964a393641cd446606ef918205f2ff5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:22:18 GMT
ADD file:f1ca2b90268fd790612e08e0e01b5ea1b63749dbec2ebb79b37a6168e5e82815 in / 
# Fri, 11 Dec 2020 02:22:20 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 08:11:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 08:12:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3354b3972c3003db2792ea643d0250983d6938232305c0bd0b2f3f8ee458c9ca`  
		Last Modified: Fri, 11 Dec 2020 02:32:03 GMT  
		Size: 48.7 MB (48731592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab97db610a1c905a0eebb8e725d651de6230d65856718b02a7b163ec6be47d`  
		Last Modified: Thu, 17 Dec 2020 08:50:10 GMT  
		Size: 7.2 MB (7201642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db3c64e92e3b49294d9851fd87b5a747ba682105ffa349b1b91e08f977d2a7`  
		Last Modified: Thu, 17 Dec 2020 08:50:10 GMT  
		Size: 10.0 MB (9974261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdba5ff0958089b4a9eb1ac55908b6ad830216260bd4f77573aca9e88494657e`  
		Last Modified: Thu, 17 Dec 2020 08:50:34 GMT  
		Size: 49.6 MB (49588839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ff7f381658311f7744c5f1782ba8c26d78918d2d55cd889f63a45f898dcc4c14
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124356930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8864850c7c7d6193c45a8e1e415574c9a9fb9de9e76ecd2c3dc8d537f7638b04`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:44:38 GMT
ADD file:8b5c11cc7a49f4bcd4f99db7d2c343338d9930a8254ed6527ec04ee8f41446d1 in / 
# Fri, 11 Dec 2020 02:44:40 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:01:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 10:03:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:452eaeaea0dc38e36d92c42c3301a9bf90cd1779fdbe05d762ba387c5823b66d`  
		Last Modified: Fri, 11 Dec 2020 02:51:52 GMT  
		Size: 52.0 MB (51961868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0d52d53c53e183980fe740fce73a7c89f32b4adea4989c49be8a76c2999c75`  
		Last Modified: Thu, 17 Dec 2020 10:36:06 GMT  
		Size: 7.8 MB (7769932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd2421bac8b34a287e63b8037ea012d6d3cc94f585a8661e2c6ac8b3b643cf6`  
		Last Modified: Thu, 17 Dec 2020 10:36:06 GMT  
		Size: 10.7 MB (10653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b747c34e3bd0d2dd82a55e6d50f5f15bddf4acd3c3a008ffcb20ac74c983fe`  
		Last Modified: Thu, 17 Dec 2020 10:36:33 GMT  
		Size: 54.0 MB (53971214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5f84293e659edb82b96442b007c7e86e9c5a1de628be2f12622a260039cfa96e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128414908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffe9737cc49718c1e8aeac652b3161aed1f55e2bdb6ff14688fd4b81154a36a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:21 GMT
ADD file:b10b66385eba9f330914811c1ea9830c75a7d222442b3076a102c918588f96cc in / 
# Fri, 11 Dec 2020 02:02:22 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 08:06:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:06:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 08:06:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5cec9c367337182f351780e9e280bde357c303f0ca43358fc7dcbe63a9420fb1`  
		Last Modified: Fri, 11 Dec 2020 02:08:35 GMT  
		Size: 54.2 MB (54157004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfed47518c0a507801e5cbe565f2d9072a66d37097eb93c108be072d452bcc7`  
		Last Modified: Thu, 17 Dec 2020 08:22:55 GMT  
		Size: 8.1 MB (8082025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c73ad66a61af03c90dfc68fd0342e7c31aede5c056cec3bb18195e6c3af97ff`  
		Last Modified: Thu, 17 Dec 2020 08:22:55 GMT  
		Size: 11.0 MB (11031118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b17636990e83105666693f7637b7aeb56bbcfc13e62b0eac8d8e8a78c158b8`  
		Last Modified: Thu, 17 Dec 2020 08:23:33 GMT  
		Size: 55.1 MB (55144761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9d5c1f923262024f9b727e14d9aa8327cece1517c640c93de80c5a775fde5a2b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122498658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:703dc26b87ef1a7188eb8e31a4fbee842d9f726a211c1f0a88c77ad008c9a8e3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:20 GMT
ADD file:1c9d3b0dae65df3d925c78ab44bc00642c930f3deef925694dc0c1a3213de35a in / 
# Fri, 11 Dec 2020 02:02:21 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 02:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 02:08:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 02:08:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede4ac036d71d6e9539de8a220d9f79c46f7c9cb9bf53f8498188327ec302195`  
		Last Modified: Fri, 11 Dec 2020 02:08:06 GMT  
		Size: 51.8 MB (51829610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6b5a1437a4f1692906f39eec85d6b3bb70a1f4164e324e1d9a001d903c7e87`  
		Last Modified: Thu, 17 Dec 2020 02:20:48 GMT  
		Size: 7.4 MB (7428942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c3593042d91d6e96d4f41313ca6efcc8a059da9d708b31e0f3dc5ebd823ccc`  
		Last Modified: Thu, 17 Dec 2020 02:20:50 GMT  
		Size: 10.7 MB (10656677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ceb1263972938cd1bc3132438877816eb79dd7894295e23b3a307805917fd3f`  
		Last Modified: Thu, 17 Dec 2020 02:21:44 GMT  
		Size: 52.6 MB (52583429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:54fc6c5a91780d4fff234cc0aee4e8810e62e414a8288d4f6efa89d22b9045d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (134964366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70ef9a50d2a580be5b1343133cac66690d1e07b6d0efe167d1fe02700fca9bba`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 03:31:53 GMT
ADD file:9583240ab6aa83a5f964dedeba18905486e879b1839d8329fc20f91cfccdd8d1 in / 
# Fri, 11 Dec 2020 03:32:06 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 19:12:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:13:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 19:14:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:018083dcdb1846644d37fb03ece4c9beb51dcb25f9851d01fc02f63c6fb143cc`  
		Last Modified: Fri, 11 Dec 2020 03:40:16 GMT  
		Size: 57.1 MB (57079148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a764e770549a2e9fcf1a37155cdeabec6a1bbe84c9873e18d51d8d1c4b6228`  
		Last Modified: Fri, 11 Dec 2020 19:50:33 GMT  
		Size: 8.3 MB (8342665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e75b76e059bba32797a570fe56ef47061e3ab409a710a1e409d2f231adaea9`  
		Last Modified: Fri, 11 Dec 2020 19:50:30 GMT  
		Size: 11.4 MB (11421077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316286b554fff880f9be84885643662c6077dc4f49c3c6bbcdd4419ed1157d99`  
		Last Modified: Fri, 11 Dec 2020 19:50:59 GMT  
		Size: 58.1 MB (58121476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5bdfbea972ccbcbd52aadc000916c9b5b5e850f0ec684cdb108ec9680f6f9314
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123090736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d034cd48130a30ccd72cfc35019a0880e0cdbe7f19e219b90b8815b53a06dadc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:03 GMT
ADD file:74a0f68651d74636caec45b24b97289c444300a4e20ead2e9dd4ecad9a89b149 in / 
# Fri, 11 Dec 2020 02:11:10 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 11:07:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:07:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 11:08:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8c1102ca26cfeafe4e6f6b885fc1f8b1c19daafd157e556c9eb528d215f3ec2a`  
		Last Modified: Fri, 11 Dec 2020 02:16:10 GMT  
		Size: 51.7 MB (51656809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12f7e9486693eeeb90ca681816ec85fe5b3711fecfa8135127df223787ae321`  
		Last Modified: Thu, 17 Dec 2020 11:45:01 GMT  
		Size: 7.6 MB (7583470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3570bdaa2dbab5cd55b00748ab7c276c7f1644555be788bccaa538f9ee606a6`  
		Last Modified: Thu, 17 Dec 2020 11:45:01 GMT  
		Size: 10.5 MB (10525427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07678dfd6cd3af2aa29333f3da97482a64670de63bcfb4f2a8331a63a7555ddd`  
		Last Modified: Thu, 17 Dec 2020 11:45:18 GMT  
		Size: 53.3 MB (53325030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
