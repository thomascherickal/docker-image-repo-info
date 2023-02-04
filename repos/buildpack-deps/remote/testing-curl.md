## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:8f0700262f62281b7a5e07fbb6d6d800fdbc6e21cf27b4170c9795c7ab3a455d
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0e118d5add7e5e58a8d31a92fad260ab990ab5a2aca9862504f9d6a37230aaba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69430870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebf911cde607da5da451b1092d4ece8b7dc5466e572d5c19870b2926f7746c4a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:50:57 GMT
ADD file:59c477049f0246331c6723687b7f8995e7a8946172b967d10fb8b67146220c33 in / 
# Sat, 04 Feb 2023 06:50:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:20:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:20aeb9ca89f41415a92cd1a5e9ff6c0280e09a250e0f950c9df57d97b0d3efb5`  
		Last Modified: Sat, 04 Feb 2023 06:55:19 GMT  
		Size: 49.0 MB (49043016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd16dee5feec7a2da71bdef1f07b5a546389f1554d69d474530b8f847d0c1890`  
		Last Modified: Sat, 04 Feb 2023 07:28:22 GMT  
		Size: 9.0 MB (9033132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba40466925cfd251e3c9b97a519794ed3580ca83f2135be0ccea17e5b2d6f99`  
		Last Modified: Sat, 04 Feb 2023 07:28:23 GMT  
		Size: 11.4 MB (11354722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ee91b555e0c3d859e23bee2690f9a7c65fc6da77913ac801c7f7b196ad65668a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67476441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ffd74114c41458d50fa4b15e86e7b850cd93264a6cf35ac89bdee76eaac8dad`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:45:51 GMT
ADD file:6283625dd02e5a15e67c45fb0ce9fec384c9086563a64fbd85ef7eec12283466 in / 
# Sat, 04 Feb 2023 02:45:52 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 03:13:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 03:13:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8a4b4311a2a6055167419fac8cc987d97e7a797e53f6176ee2b5d0e6edbde230`  
		Last Modified: Sat, 04 Feb 2023 02:50:25 GMT  
		Size: 48.0 MB (47993284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35559dda00a93e84323ff0a3cd944fd9cebe193cb866743b2bf5d33ac8f7ecd7`  
		Last Modified: Sat, 04 Feb 2023 03:21:50 GMT  
		Size: 8.5 MB (8481336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dbad85bdc4db8aa9aaa97d1620037878a7830e27a0a13e6913172f0885cba0`  
		Last Modified: Sat, 04 Feb 2023 03:21:50 GMT  
		Size: 11.0 MB (11001821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:84ee21501749781dbc056970675637881c81c2a73414be2499a33fa93ff2446e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64554730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4207e2320e656fd28577d92647f6148a1d53c3b15ad70fed4a25c7beed75121d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:58:46 GMT
ADD file:7fa388eb21c424f9b3d978f277c454b5cb8a4c4fc0dac864298e9cf12161b132 in / 
# Sat, 04 Feb 2023 09:58:48 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:46:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:16b554b0ae696936d2556c56490dc1cb7af234f9a415a93932213ba90d19bd85`  
		Last Modified: Sat, 04 Feb 2023 10:05:12 GMT  
		Size: 45.8 MB (45794144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37939da9cb6c3ba4566c2d20c05dee5ec7361c07649557a19b8e8d844ef0cf4`  
		Last Modified: Sat, 04 Feb 2023 10:57:57 GMT  
		Size: 8.1 MB (8124732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d72a01582fa10ad6cbabe8e802a8e57b4fb57dd818ac7cf92815d91a6a0a55`  
		Last Modified: Sat, 04 Feb 2023 10:57:57 GMT  
		Size: 10.6 MB (10635854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a8e7ab1b2708a0629786032fa2204f66e7934e6e4a2bd36d4ddcb9b06efd6da9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69266931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd8f10a65cb048212eaae7bed0da3019c1f04fd7e0c4d1d6bde90952c8c4b37e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:43:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:43:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f6dd523027aa16778d661d27e72bbe882cc841d9a40bcf7ba993f9653c66e5`  
		Last Modified: Sat, 04 Feb 2023 06:51:08 GMT  
		Size: 8.9 MB (8865599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef33a1f8ffdb43ea2d51e44c388d4de6bedede50060c1397f6ae0eff23cd307`  
		Last Modified: Sat, 04 Feb 2023 06:51:09 GMT  
		Size: 11.3 MB (11319794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c742b52cd8819fd331e1aefd6ca10357d9f82a2ad366203b315916ec5ef4b3f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70862551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a28b04959dca1868f3e0ef10efe24177f0a97a3c1472b49f3eec8f388d33ddb7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:48:40 GMT
ADD file:71f93fd08314b2207fb2e5840185c4db4279fa8f008742cf35eaf4daf925d475 in / 
# Sat, 04 Feb 2023 07:48:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:17:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:17:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0b6e1871a6864b2026696c7ffe48da3030a97146a6a0f3ca18f87c19b1ed6e05`  
		Last Modified: Sat, 04 Feb 2023 07:53:55 GMT  
		Size: 50.1 MB (50093420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7274669ca31ae25c99ffbeb62b7bf63cf6e70c0afea787b6483e8e1e233d5`  
		Last Modified: Sat, 04 Feb 2023 08:25:56 GMT  
		Size: 9.2 MB (9211501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222e731d14a700e618d6e7298602f00a0ac9884fbe12a867349d9a13ae14bb4a`  
		Last Modified: Sat, 04 Feb 2023 08:25:56 GMT  
		Size: 11.6 MB (11557630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6cd0fed88f490f50866d7504b3a97b6a3fb67d6e58e00bc85df826ab69842c5f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68545314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9bb5376bf033399b2da084a6eb123432acad4bba50dad44cac1d5b0dd74ff8a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:13 GMT
ADD file:342f09d1a542544d0b028faf681c7e97bab2676412290d4af1ab83b550eb0404 in / 
# Sat, 04 Feb 2023 06:18:16 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:28:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:29:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:811d77d1a16ee11b725d10eee34b4675405052eeace5043fea40862dac9fd740`  
		Last Modified: Sat, 04 Feb 2023 06:26:25 GMT  
		Size: 49.0 MB (49040889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafe731118197b5c6270a970451012408dca08211806ef6c76de0197dc4f22a8`  
		Last Modified: Sat, 04 Feb 2023 18:55:35 GMT  
		Size: 8.4 MB (8398884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c759c150dc8306fa76a100d6e285e0915607f68c337e5c8945cda21cd969e07`  
		Last Modified: Sat, 04 Feb 2023 18:55:35 GMT  
		Size: 11.1 MB (11105541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:93e952515c73f476625c5020115ccafc88412ee1604f1a05aa054c5b0c12be7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74794735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97cfaca978966ac322b03efbd8c567a86396a13dc8e706ab3410be6906ec21bc`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:24:35 GMT
ADD file:75252aac3ef2cfeb95bfa5e27d34d7632e938a4cc508e662b033aebb438bf9ed in / 
# Sat, 04 Feb 2023 12:24:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:57:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ad7bb1bf81ba24a5e75d96e5759bfa08a04cf654eda26010b8b1bdd6eead92f2`  
		Last Modified: Sat, 04 Feb 2023 12:30:47 GMT  
		Size: 53.1 MB (53066627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a43d91cb4f1d38d440125ef18b21ed870c9dcca915dc7e20243430d8adac5f`  
		Last Modified: Sat, 04 Feb 2023 18:12:46 GMT  
		Size: 9.6 MB (9613419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42696410cee2c14decf6673c1f2af21d8399af5087bd8d0a8aa5836b6eb83e2`  
		Last Modified: Sat, 04 Feb 2023 18:12:47 GMT  
		Size: 12.1 MB (12114689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7bc39b1b456125db868bbaf2e28245d9c4cd26f1c438e846a8152f4fd67d18e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67314349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2cf598fd426bf6ea539f44659ac323e40efde9c58a4bc0d02b0861bbd656763`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:05:23 GMT
ADD file:cac3f762206c0f8ad807211cb73145ac093d8917f5b8cf3a79eea3ef1fd14eea in / 
# Sat, 04 Feb 2023 04:05:26 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:30:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 04:30:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5788bb4f4cdc5bb0c03495b0d17914750f0dffcbdc053321669358a95967dbed`  
		Last Modified: Sat, 04 Feb 2023 04:09:43 GMT  
		Size: 47.4 MB (47429742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1e84e5465158af09efec27ef891007b9bd6994985807b81f054e6b39a0cdf0`  
		Last Modified: Sat, 04 Feb 2023 04:38:50 GMT  
		Size: 8.7 MB (8666425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1fe479ceec98fa274b9f162d0d9d0a555e7ecadb9aaa64ad94b2423e5d22a1`  
		Last Modified: Sat, 04 Feb 2023 04:38:49 GMT  
		Size: 11.2 MB (11218182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
