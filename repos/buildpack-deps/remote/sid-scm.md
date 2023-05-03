## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:9e7e69c94acb70fcd61de8e876e7d2bed6f20bc43b84d8fd0c2335a8a5009ce1
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
$ docker pull buildpack-deps@sha256:e98f4fe9de23a7fcb3cdd8a541780d25868969254edfbdc6b684b43f107cc17a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134030233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8398408c914013f92f2221b216002eb5e49a917e6064fae74dff990c81da3b34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:55 GMT
ADD file:0936f6fccda991ba27a7f73ca61c23a436b7ca417e504b66d5a68f2283e1e81d in / 
# Wed, 12 Apr 2023 00:20:55 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:16:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:16:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:003dca91ec623536e08abc4e1bb2849836a84c44f82e24b97fd5423162a4d46e`  
		Last Modified: Wed, 12 Apr 2023 00:25:13 GMT  
		Size: 49.3 MB (49287652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871d61b23314698ce4b5e4e3296e774e003e0209a9f4b5d6a1f04093f5e1d366`  
		Last Modified: Tue, 02 May 2023 23:40:48 GMT  
		Size: 20.2 MB (20237190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff64add86932cc6262662d13a3e82ad4baa2d1399c2e0558f1557c45bf1edea1`  
		Last Modified: Tue, 02 May 2023 23:41:04 GMT  
		Size: 64.5 MB (64505391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4fbd04dc532fef9510fbca2684a0cae905d90b3632a837b1464936e01fa51bf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128637921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701a4eae563704152ff94e807feb0af336822bb10dc696b8dee2f911018e401f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 22:49:00 GMT
ADD file:2228a07c6ec82db1e0719684d77cecf448c3be947c2b1b48347ba5de9e5b57f8 in / 
# Tue, 02 May 2023 22:49:00 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90d5a5fdc15637fce928afc279fecd9adb82fe3c476f174458fc6bdd7fb4b57e`  
		Last Modified: Tue, 02 May 2023 22:51:47 GMT  
		Size: 47.2 MB (47167062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d5ead8dfbbce713a49ce8b7288e71d62ed89f8fe7bdc5a9a3601fedc95d026`  
		Last Modified: Tue, 02 May 2023 23:05:01 GMT  
		Size: 19.3 MB (19334073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7796655abf4f2957cc5d94738416e24552291e28456a70d36d096584ddeccb6e`  
		Last Modified: Tue, 02 May 2023 23:05:21 GMT  
		Size: 62.1 MB (62136786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4ab7baf06999a54f07eb1c5030b4e0375a3b9a8748ffff33c0764d1baa8a80a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124256400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0ab824f3581a9ce7bfde26c1471e8f8e8a5c0b8262e64eddd468cc9c2a7079`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:33 GMT
ADD file:f8bcd71f10e7adad706b3a1685fd5c4844e3ebde65bdf9a7c004d7b9dd3520d7 in / 
# Wed, 12 Apr 2023 00:00:34 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:05:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:06:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b0aac501774f41dc4e46815077e011ed06b86d9469c6ca28755965123669423`  
		Last Modified: Wed, 12 Apr 2023 00:04:46 GMT  
		Size: 45.9 MB (45890234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40f36cc9abf83398d26c55cfc4ca06cc31dcf06c33d2c7da24b80a00c57a974`  
		Last Modified: Tue, 02 May 2023 23:38:12 GMT  
		Size: 18.6 MB (18602339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd64b39b95dbe081b6e8dcc7962f63ba1863cd81c23a43d9e0bb856367a18b8d`  
		Last Modified: Tue, 02 May 2023 23:38:34 GMT  
		Size: 59.8 MB (59763827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:040237fb66325aa0911aae7bf278a04197ca17823259f7b763691fd1dea72cc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133850179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfa3bf95632a33ccb6b2dc7440c26817d1ad4da9c60332d9977462e8ff87f7e1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:21 GMT
ADD file:2784bc6dba1e1dbea293e074ebf51fa7d89cb5545ea63ba2ed75b74d067387d4 in / 
# Wed, 12 Apr 2023 00:40:22 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:44:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:45:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43d214f7ab3ca35a0c9ed4d8cdf62b36248aba2fa1bbac4ecd64e82ba2520b70`  
		Last Modified: Wed, 12 Apr 2023 00:43:58 GMT  
		Size: 49.3 MB (49327656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5d7b5b9c3f7e79362c5949189b82ea6d0b2dc70b5c1b5281c8f029d11d56c3`  
		Last Modified: Wed, 03 May 2023 00:12:58 GMT  
		Size: 20.0 MB (20035112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7432c6b3e6f3f261285ad0a5516a1358e065710a8ac6e175a4ec346fef04f6b9`  
		Last Modified: Wed, 03 May 2023 00:13:18 GMT  
		Size: 64.5 MB (64487411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:56f6fd88acdaaea819696b325c776567bc55478b33b34c1eb5e620b376fe1f65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137460958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c223207da58851ce744acc6cdf603b79681340d311e48674b08e7e4a36e191d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:47:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:47:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499e0d2794581c0b3fafbc9ce91c00afe10e1d6704447fcec0b1b4ff6df41bed`  
		Last Modified: Tue, 02 May 2023 23:57:29 GMT  
		Size: 20.8 MB (20818586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8f1e71833446e567aaacbf83081ffe5a7cf93453d6d2ed37d800c0b89c7013`  
		Last Modified: Tue, 02 May 2023 23:57:51 GMT  
		Size: 66.3 MB (66331473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e845a696a1ed61f5ad335ad083d01ee77465104e6436b617ba359805cff6f55b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132263282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1fe70e304972211e2af5b55f5c8f2fe89016c1b2d5592b07509ef05a506bcd1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:10:29 GMT
ADD file:60b5ce2a691448a1aab43387ba9337b8cc193a2cbb2a01ac71f5f0cb083415ff in / 
# Wed, 12 Apr 2023 00:10:34 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:27:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:29:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45f3dc30e8865982b1af34a4bd64597aea34350dd1bf817342cb2901014ff9a2`  
		Last Modified: Wed, 12 Apr 2023 00:18:10 GMT  
		Size: 49.3 MB (49296248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf4b724cd7bc4b197cc5156622c80e9b57f3b3c9185058f2ddc799d3f4b4cee`  
		Last Modified: Tue, 02 May 2023 23:42:14 GMT  
		Size: 19.6 MB (19554260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f568b715afffdc8179b7108b5118ba8037058e2a10fc275f68cfdcca38bb4c`  
		Last Modified: Tue, 02 May 2023 23:43:03 GMT  
		Size: 63.4 MB (63412774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aa7c997bac5324b859d8bf8ea16768a4729faa04a7ed25254e4274d85ba4397e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144819020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b03f7fdaff1fc66487e1c3c64f713b6fab9fb3ccf0a83e23418f61dd8cce7aec`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:41 GMT
ADD file:8700846eefa6ef0670106ef8055671479d597d057ee34d1d248dbefa5977753b in / 
# Wed, 12 Apr 2023 00:08:44 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:28:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c14c235d79599f644d6f952e975871669fe8a00e0434e5d26966f11cfb3820b`  
		Last Modified: Wed, 12 Apr 2023 00:13:39 GMT  
		Size: 53.3 MB (53291710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f7fcb97c8afc6c0c2224ad25838f0b2c58a23b8b1ea868b93f7b075fdfd416`  
		Last Modified: Wed, 03 May 2023 00:14:32 GMT  
		Size: 21.6 MB (21578703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726c71ee2f84a020202671d9a1b2e9064700ac60dcf19b2b863286996fd0ef79`  
		Last Modified: Wed, 03 May 2023 00:15:00 GMT  
		Size: 69.9 MB (69948607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:2d5d68cca9dff91db89ab5f1e95fc64d8faca9d5016039c8eda4a73f4beeb2fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124123862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efabf2c6cb01c282a4d5cdb13d5c81297b8d421f16cb94af29eceb39e3193e5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:29:17 GMT
ADD file:4e365b380d9cfb77573624c399d3376d19fa5c7028c44b681071b426fb1c6db0 in / 
# Tue, 02 May 2023 23:29:19 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 May 2023 23:54:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29b183cb384ba20db9a991d4213be72a43fcec3d5fc87f259bd5719d35027d1b`  
		Last Modified: Tue, 02 May 2023 23:32:35 GMT  
		Size: 45.5 MB (45510102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93940bc329d1d971861f44e84f01d2bf1b1b0075644023b2caae44992f0e70cb`  
		Last Modified: Wed, 03 May 2023 00:03:11 GMT  
		Size: 18.7 MB (18656704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9b13ea8a5a6cc6efb43a7b1b940dbe6a4cf4e6dfd3a66e0d926891398ac6c`  
		Last Modified: Wed, 03 May 2023 00:04:32 GMT  
		Size: 60.0 MB (59957056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

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
