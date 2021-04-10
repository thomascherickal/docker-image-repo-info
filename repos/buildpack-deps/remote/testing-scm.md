## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:1a23db5d05508d3ddff48ce233b299ecffde8d6125a48add8a06058dbe950388
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
$ docker pull buildpack-deps@sha256:ba62d0a2b0f3696140d8cfc9b555ffdbd0f2ed59dacb089bfd46adac79252d61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125451306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de05919903979f6602d333781a7e38a9543fb42b8a0946f7d99495b7abc4281b`
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
# Sat, 10 Apr 2021 01:53:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f7ac119459a7d1a89ed94746e1639c3afde989102e0ea3a2ed86a6809bedc599`  
		Last Modified: Sat, 10 Apr 2021 02:00:58 GMT  
		Size: 54.6 MB (54564714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1189357f82628653cc8bf7b1af02f2bff5a5f7ae86e9dbf31dacd6eb9e2be6a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120346466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e2b69f7678a204d15073c390ce2db7b7c16e691f7379cb8b1c3070b9798e320`
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
# Sat, 10 Apr 2021 01:58:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a97efcbda3f28c049d797110675f9955cc21e80b07bfcd8bc66e52d49802739a`  
		Last Modified: Sat, 10 Apr 2021 02:17:54 GMT  
		Size: 52.3 MB (52314013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4d42e40a5aeebd099a59b9532641fdf18084c0a4e69d7db01872a607322290e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115537221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd679ec1a51c5e60ec3ef8c9926f411d290f511fd775c27646fe4bb4fadb96f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:58:24 GMT
ADD file:5e17f4d5cdf1ff091554ccfa33e22ab2be0c278b0cec1c11b45333deda2cfc79 in / 
# Sat, 10 Apr 2021 00:58:24 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:01:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:01:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 06:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df95183d3a18fe92c278757657c6fef8fcc11f2a9a578df2f2b00dbccf0a8ea6`  
		Last Modified: Sat, 10 Apr 2021 01:06:36 GMT  
		Size: 50.1 MB (50070347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156c39bdbf88c4fe691e2b8db9d8884ace98a295e72db7f8f2c7a7b09d88301`  
		Last Modified: Sat, 10 Apr 2021 06:18:29 GMT  
		Size: 4.9 MB (4920554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5c1a00fb4cd0a81f72ea5458a8eb52ee825d2ec64b5b3d6324e8fe844eed2a`  
		Last Modified: Sat, 10 Apr 2021 06:18:30 GMT  
		Size: 10.2 MB (10218022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f63a9b9b58ff5c896075723b17ad5cc2bd3e1daada4e1379a89a0b57120ce9`  
		Last Modified: Sat, 10 Apr 2021 06:18:54 GMT  
		Size: 50.3 MB (50328298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:08b6a175308caf77256b1b30be4e60cc7424c560467c95950aa529937ed7b1e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124229613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9890482767a33f5d48373023c29383d2bbb6cd185365cd559de91f38e2de7feb`
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
# Sat, 10 Apr 2021 01:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:607f59eaee90bc16e7091c941cb4640481bec283086c165c038bc666c6072d4c`  
		Last Modified: Sat, 10 Apr 2021 02:00:00 GMT  
		Size: 54.7 MB (54666062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:425f07a543fcc06f8b48fe4b169f4bb4966e4987f8f4a91df35ba31accd802c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128319506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79e7190569c06cb269bc6325858a9bcc24772b24b372032b5ca4bf1cfa9f3749`
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
# Sat, 10 Apr 2021 03:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1e044730d7057c92a5b5235d54b58ae32454dfaf5781ca5e0f7dd728dae5dfe2`  
		Last Modified: Sat, 10 Apr 2021 03:28:28 GMT  
		Size: 55.9 MB (55908848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6e4f626ec7ae98c033861c9fbdc0af9dadb33f6b799bf07a7f6429e72c0ef23c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122410242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59ec203a1937a34c483e08fc5355004817d8421d4265b1c0eb648cfdf6ef0b6d`
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
# Sat, 10 Apr 2021 02:04:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ef31236e593348d8cd737733087e3c6eeb0c8440f32d9c3b46597be1b4e27dba`  
		Last Modified: Sat, 10 Apr 2021 02:16:18 GMT  
		Size: 53.3 MB (53299532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:129ac163986f1d7c1a449d132ba28b99270e0a264a65758d649a386baf118b5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134649324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a278395be452d203838d7f68ce0976bc81f8f2fd06ed7a50e6fce60c200837da`
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
# Sat, 10 Apr 2021 02:00:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:17976d558c617922225b59acaffe6c7bfb5a5777d4e19401af2bbc1479562c32`  
		Last Modified: Sat, 10 Apr 2021 03:03:28 GMT  
		Size: 58.8 MB (58846965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6f654998d1d53fc6c3536b199dfd2d595f3cb586ae0cd8d2b2e1f0c5f99ba921
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123079535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d04d8d789ab03f48a29d4b8b0e5cd2e9be66e8809a67b257dd1bb1958e9ea3`
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
# Sat, 10 Apr 2021 01:25:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a40ef89f997c44974926e4fae492c195e0b73cf29dd614681b270cc7c5def582`  
		Last Modified: Sat, 10 Apr 2021 01:33:01 GMT  
		Size: 54.0 MB (54038719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
