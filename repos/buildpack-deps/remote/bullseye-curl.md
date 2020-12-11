## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:33b9e56d03ff25865c86c52e29b719626ac098e123318020e752d2b72a4674a5
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:52a451d75736d9637660bd8a9af1af091343a1b64c89f7b1042f43451afb61eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71652979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855ed4dd0332982fb0d69380d5fe40085b19dd27bfb0373f94afad49e5eb9c3a`
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

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:897b5d335b50f8f827406c9bf00b17538a3ff0a6f96d95800e73b29738b1af9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68832602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0348dfcc6358135a5d06efffb7e062639f0a5f0771ad750dbd22f7e488c05971`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:8b9117df3f1a986438250b725bc8ec117cf1caba2e6953cf9a870edbcda4c565 in / 
# Fri, 11 Dec 2020 02:03:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:37:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:38:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:69233e69b29a579de45732361ee762ae02ccbe96b0f2a09fc2a48a802a25b265`  
		Last Modified: Fri, 11 Dec 2020 02:13:31 GMT  
		Size: 51.1 MB (51053259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d208cbc2dd055b46a0eb797352719db7e40a64bb90bab94b3d64b5b3b1c4a6bf`  
		Last Modified: Fri, 11 Dec 2020 03:04:31 GMT  
		Size: 7.4 MB (7444057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8ae15eeacf7f92e597567cdb02de06832bdbbcbbc72e66d77dba4a1854f649`  
		Last Modified: Fri, 11 Dec 2020 03:04:34 GMT  
		Size: 10.3 MB (10335286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5cfdf9815c7d3d828049ed1a854203b6f81c26073f4ba85dcf94eac7d9f61470
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65891642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c4e75c19f8c092c63ac3fd6ea200e9f5aac0587835b94aae8ac6bd5864b62f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:22:18 GMT
ADD file:f1ca2b90268fd790612e08e0e01b5ea1b63749dbec2ebb79b37a6168e5e82815 in / 
# Fri, 11 Dec 2020 02:22:20 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:18:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3354b3972c3003db2792ea643d0250983d6938232305c0bd0b2f3f8ee458c9ca`  
		Last Modified: Fri, 11 Dec 2020 02:32:03 GMT  
		Size: 48.7 MB (48731592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f0027df82d0578bcc2d43af7c68680af181d153ad76b785b97e3ffb1a53e8`  
		Last Modified: Fri, 11 Dec 2020 16:41:21 GMT  
		Size: 7.2 MB (7185940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce3f21be10a21df5869d3131ec5a4c6715acb9e45fe541b0050baa4013a18f0`  
		Last Modified: Fri, 11 Dec 2020 16:41:21 GMT  
		Size: 10.0 MB (9974110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:31bd121faa0eed85f620e127d44bb25795a0be8389a88a46ec1b77df6cd179c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70368483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b514bb81e804e4eaa3d8ac6364e67015310156ed5e0f84342247538ac7705cfc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:44:38 GMT
ADD file:8b5c11cc7a49f4bcd4f99db7d2c343338d9930a8254ed6527ec04ee8f41446d1 in / 
# Fri, 11 Dec 2020 02:44:40 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 18:48:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 18:48:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:452eaeaea0dc38e36d92c42c3301a9bf90cd1779fdbe05d762ba387c5823b66d`  
		Last Modified: Fri, 11 Dec 2020 02:51:52 GMT  
		Size: 52.0 MB (51961868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a365361933f85eda3c750d50aca8a81a4775d22e9d737de3c7c45bc6b95a3b1`  
		Last Modified: Fri, 11 Dec 2020 19:05:17 GMT  
		Size: 7.8 MB (7752728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e4be3f3b3a66559755e4f49afd8b36b637ff6ae027a2cad951ec7f639f34e8`  
		Last Modified: Fri, 11 Dec 2020 19:05:17 GMT  
		Size: 10.7 MB (10653887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9b42aeba95f13469f25f67be2e71ce363274408dfef25e30a08001a4fea58351
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73249987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e850684217c2a9d3762afb430ef1373622b7b7e07903802326ec16d8be823528`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:21 GMT
ADD file:b10b66385eba9f330914811c1ea9830c75a7d222442b3076a102c918588f96cc in / 
# Fri, 11 Dec 2020 02:02:22 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:50:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:50:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5cec9c367337182f351780e9e280bde357c303f0ca43358fc7dcbe63a9420fb1`  
		Last Modified: Fri, 11 Dec 2020 02:08:35 GMT  
		Size: 54.2 MB (54157004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0adc7b066b08d37e3ce68b7d917336758181b23bb781ebac0c7df6edaf47c64`  
		Last Modified: Fri, 11 Dec 2020 21:59:40 GMT  
		Size: 8.1 MB (8061876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134225cc6c5191f44ad18dc206836e52539c5e5efc9d7a37e8e3440faa945bc7`  
		Last Modified: Fri, 11 Dec 2020 21:59:40 GMT  
		Size: 11.0 MB (11031107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2fc7826d2e79f99aec73fc7b74f6d96c7e395355a5547ce36055ce341dac31b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69896403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a586b56028e0342f33b0f712a36ebf1db7dbb876bb1923bd701cb0b5e72614c8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:20 GMT
ADD file:1c9d3b0dae65df3d925c78ab44bc00642c930f3deef925694dc0c1a3213de35a in / 
# Fri, 11 Dec 2020 02:02:21 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:44:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:44:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ede4ac036d71d6e9539de8a220d9f79c46f7c9cb9bf53f8498188327ec302195`  
		Last Modified: Fri, 11 Dec 2020 02:08:06 GMT  
		Size: 51.8 MB (51829610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97d6058f001d48012d3119e7be581954924dd50d584771418ffecb191be4d2`  
		Last Modified: Fri, 11 Dec 2020 02:58:53 GMT  
		Size: 7.4 MB (7410105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5e05d9ca9fe9992047f5f69faf9d8cc20423eba1ebf9226cd16e85d820255c`  
		Last Modified: Fri, 11 Dec 2020 02:58:54 GMT  
		Size: 10.7 MB (10656688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bd51855ef1f998eab3823d63bc8490cab44521d2969439ebb0fd6998b5adee9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76842890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec93074e3818ecff950b252f2768a81101a42f703ef9aa4b1d9a9b09888ee7a3`
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

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9dc21b1f37b5a6fb37f56babc3fd41e7caec2a3f3edd99eab2e0cb23776795e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69747970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03c89d470a2c75bad62c51b40f40be64d1e5b6d565d9cad5f13242a6bce0eed0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:03 GMT
ADD file:74a0f68651d74636caec45b24b97289c444300a4e20ead2e9dd4ecad9a89b149 in / 
# Fri, 11 Dec 2020 02:11:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:56:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:57:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8c1102ca26cfeafe4e6f6b885fc1f8b1c19daafd157e556c9eb528d215f3ec2a`  
		Last Modified: Fri, 11 Dec 2020 02:16:10 GMT  
		Size: 51.7 MB (51656809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5318fd9b9f903620dcea8eebe0d1b3e4c22fbc8b859c0bf46ac13755d1a52a`  
		Last Modified: Fri, 11 Dec 2020 16:14:25 GMT  
		Size: 7.6 MB (7565720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845cbfbba3746772baf57c643c9a8edde11b111c4a69407f278d0c47ace4f158`  
		Last Modified: Fri, 11 Dec 2020 16:14:26 GMT  
		Size: 10.5 MB (10525441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
