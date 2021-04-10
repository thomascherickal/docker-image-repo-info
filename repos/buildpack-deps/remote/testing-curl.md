## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:db6d3a649c69b424dc0a318f00850f6db949b28b02ac65502493de0004e273bf
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:84c95f56515bfaa57f8951146756e4cda20a6037dff18d4779b2619ff0549687
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70886592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86314b2dd41db3d24b7326f31507ad5a2ea4fcd1b4f8a54c646d0b3063644c0d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:19:44 GMT
ADD file:09ffbc0a4ab7c70a3071740e19113a2f2d61593241bfb8455aeeea7877b8784c in / 
# Sat, 10 Apr 2021 01:19:45 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:53:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cf7e31f852204930ef60bd4c12f9606812c0b9ba6235e2e46e1a5900f2db9d30`  
		Last Modified: Sat, 10 Apr 2021 01:23:56 GMT  
		Size: 54.9 MB (54868257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6dc39acac51e10c09aed5f7835e7a99a2a9680be75d2352924fdee6a2f744f`  
		Last Modified: Sat, 10 Apr 2021 02:00:36 GMT  
		Size: 5.2 MB (5151329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450329263cd7b5d35ad44c880afbb2268b05ee361a4ffb617cc58d422bec81d`  
		Last Modified: Sat, 10 Apr 2021 02:00:36 GMT  
		Size: 10.9 MB (10867006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fb877bd703cd3717a9cf89d87ea16b1bdb55e16d7a2ac50b9a689a47a0e1f755
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68032453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24a93f627b9b872d8968d2490751b27c86f91102855d945f0ab837d7d6becae6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:50:12 GMT
ADD file:37fd08ef57f840011e25ed9f68d8b5197a5378b1f7bebee7fa587d5e7d561844 in / 
# Sat, 10 Apr 2021 00:50:15 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3c6e089fcab6bbe7eaacf21e4d0c43c7da8b8a21cad425a714fbb8d6798ccadc`  
		Last Modified: Sat, 10 Apr 2021 00:58:12 GMT  
		Size: 52.4 MB (52401447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ee67814b7dcf0dbbde45ef110cd1fbd3dc8c7c55ffa598f8877464399c4a6a`  
		Last Modified: Sat, 10 Apr 2021 02:17:23 GMT  
		Size: 5.1 MB (5061154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1690c9d4b9ea482011659d97a74e3b027cd75da0bee59c2fb7cf804c749aa`  
		Last Modified: Sat, 10 Apr 2021 02:17:29 GMT  
		Size: 10.6 MB (10569852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a8cc33910a9d93ba8710a438f09d6bd27b81b9acd4c12284218df462be810ec3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65208020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680cba8daf8017deaff704862df3889453a80b8af436c03f497a3109bbc58d86`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:07:05 GMT
ADD file:81d46e360628ea35bb1ec870f07ccb5c7722c2af2296557ac007f32663ef1cec in / 
# Tue, 30 Mar 2021 23:07:09 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:18:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:18:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c62a7336a784ff2e5eceb7d0da019a0022517c331efaef6fb92eca67135c6ac0`  
		Last Modified: Tue, 30 Mar 2021 23:15:13 GMT  
		Size: 50.1 MB (50069202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5e37c5cf7fe4b128b7450320e29ce9023508d8710e2e020d7e16f2f5c8db48`  
		Last Modified: Wed, 31 Mar 2021 01:35:02 GMT  
		Size: 4.9 MB (4920655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a0d6ba1227e34af56c86a1a156db9127d0e70b920d2ad598b3f031d3b7190e`  
		Last Modified: Wed, 31 Mar 2021 01:35:02 GMT  
		Size: 10.2 MB (10218163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e55b9bfc3ccc4190f2adf5f1c4ec1028d49c0cb7a686a16506680081fa28fefe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69563551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c6a96c1d1126a8a567c637d37ca1f3a60e4aa760ae710eb5770971ea6b2871`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:14 GMT
ADD file:e1b7ed0c35932136d6c29369c3eb387896a482b3b227f18462715ed1690af4d4 in / 
# Sat, 10 Apr 2021 00:40:17 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:43:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:43:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a5ad85c1142d6ba07dd2031cb0c6c7513422a29a4e0446b232121280077ee9eb`  
		Last Modified: Sat, 10 Apr 2021 00:46:54 GMT  
		Size: 53.6 MB (53555409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cf7b2e11a6c2d24640e32bab162f44730583fd12321a0b43f568de4528c6a0`  
		Last Modified: Sat, 10 Apr 2021 01:59:38 GMT  
		Size: 5.1 MB (5140721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da257970ac9fb41c862a9ea5857f77aa158778d568d6766498b801a239be01e`  
		Last Modified: Sat, 10 Apr 2021 01:59:39 GMT  
		Size: 10.9 MB (10867421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ad950ac6a56d9ee8e97abb6dd3cd544a72d02a7de4cc9046574e6902c2b45835
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72410658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30de5e8214e0549e72653cdd8a9f84b621dca4d0358f88c248520845184a1cb8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:38:57 GMT
ADD file:72806e483423c962f867acf22783e8b91aa9d8486d1d35505eaa5442df41be57 in / 
# Sat, 10 Apr 2021 00:38:58 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:15:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:15:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c73c775bc05dae13d9e00c5c3e6660d213997be492a06abcfe494e5fbfe97f21`  
		Last Modified: Sat, 10 Apr 2021 00:44:36 GMT  
		Size: 55.9 MB (55881380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9e0bd737226fabb79b27a428df2d8a89fad1d3d4380eef8f36ab1540f975ac`  
		Last Modified: Sat, 10 Apr 2021 03:27:53 GMT  
		Size: 5.3 MB (5280440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc93fbf8ae86f8ca0c477fd1e852305a2a6b5b121a2a0d8a6c785ab27d113805`  
		Last Modified: Sat, 10 Apr 2021 03:27:55 GMT  
		Size: 11.2 MB (11248838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:279f30bca30154b539bc4dfabba6e643b5061904c8dee19a1d5ddcfd2336d609
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69110710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98cf0c671e2645a6642755db479ce97489545402f1546691ab374fa217dbf17`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:08:30 GMT
ADD file:05ecd203b7e6783fda8a687a6d061102831b24ebff7441f9b8bd407ea76580fb in / 
# Sat, 10 Apr 2021 01:08:31 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:03:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f35fc328cfb1004badf99abc0ffb0868b98173f9361dc1a1a0fb16c971579044`  
		Last Modified: Sat, 10 Apr 2021 01:13:59 GMT  
		Size: 53.1 MB (53127395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690bee2c409ab17046d8c4a0498a7accd7ca61857eedeb2b607fe4cdf23add4a`  
		Last Modified: Sat, 10 Apr 2021 02:15:27 GMT  
		Size: 5.1 MB (5113022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f235b32aa2551623bc33d129d9bf32cc4117b27ebeb38e2cf6a1908bf1c17b3`  
		Last Modified: Sat, 10 Apr 2021 02:15:29 GMT  
		Size: 10.9 MB (10870293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7a695c6d7c42b4f52475f6457119a7fafe3c9b516db6fb5d34e739ffd2ec6902
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75802359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d6a8d229c7f6cef8da58fe6f4191533a85693de63ce9b4ffb3612862c809120`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:24:22 GMT
ADD file:c677239aef001babcb1663e8f2e9aadd81b7da6c581bb55368efc93625140098 in / 
# Sat, 10 Apr 2021 01:24:32 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ddef5f25272167da6de06606c43b7762709f7f2d95d2624ba3d2adafbd2d13d5`  
		Last Modified: Sat, 10 Apr 2021 01:32:37 GMT  
		Size: 58.8 MB (58783245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4e8fb057889bcb16e3c8b7bc0f46ac465eaad43d9ecaee96fe62ecab47f05`  
		Last Modified: Sat, 10 Apr 2021 03:03:04 GMT  
		Size: 5.4 MB (5399544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2dbcd738d9aa03edf4d9d84dad745a9d48e9f2d3eb4febce8ec5aea58e4be58`  
		Last Modified: Sat, 10 Apr 2021 03:03:04 GMT  
		Size: 11.6 MB (11619570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:12bfbe0109599fee1ae6c62fe38d1446471ee84f8ba37abf217b5c2dfdcb7b99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69040816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4736ec994253f83bcf8b00ad91ce3fb3a776e8cc83a3dfa0316e7a35151824a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:38 GMT
ADD file:5e12a744308594a409852feb52fdce1bafd5db69b42d23f30da5fd5da36c7900 in / 
# Sat, 10 Apr 2021 00:41:42 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:25:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:25:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:22dffdd7e7137fea3c673394c15d7ec19300c9ca95cda64cb366ed192a6a2632`  
		Last Modified: Sat, 10 Apr 2021 00:45:03 GMT  
		Size: 53.1 MB (53148269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db5926e54bf02d4a1b97c8037cb92e495f9b52afc71b9b1b79693fcbe59cd2`  
		Last Modified: Sat, 10 Apr 2021 01:32:44 GMT  
		Size: 5.1 MB (5134073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128ec9d2e5826957253eb7a1db9732773e779280b04208870af23a99ed5a26df`  
		Last Modified: Sat, 10 Apr 2021 01:32:44 GMT  
		Size: 10.8 MB (10758474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
