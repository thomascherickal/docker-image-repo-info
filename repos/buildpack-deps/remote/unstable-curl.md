## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:ddc8b066188159c0c5cbd2c318814295264d016b3cdda8ed5f1bd14316fe624c
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:905f9df2bde572cd8d48891b982b4e5efe1f468a2762b50637d8abfe2aea2b89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69541258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed21ed1b695005e8a7f02c2b2c926fac2d2838312178e314ba185d29e0b24093`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:42 GMT
ADD file:6261ecb921e04d2b3f6fd44e5dcb5683154bc0beee4f26913c2be9395a060489 in / 
# Tue, 02 May 2023 23:47:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae396e350f30e1defad1bfa67a84b97389d42cf3442551e39a0e2bab6b53a50c`  
		Last Modified: Tue, 02 May 2023 23:51:56 GMT  
		Size: 49.3 MB (49299270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd17d28808409b147a3bf1ad99b0f7837c93556c98e22adfd32391f10cd514c3`  
		Last Modified: Wed, 03 May 2023 20:15:05 GMT  
		Size: 20.2 MB (20241988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:eb28cafed8fb9f649b1146976aa4d394193e1ab6ac20ac5a505ad30b92936096
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66501135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f27e288b09f897f940a7a98698f8c2aeebd2fd8681de726047e72cea8289353`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 22:49:00 GMT
ADD file:2228a07c6ec82db1e0719684d77cecf448c3be947c2b1b48347ba5de9e5b57f8 in / 
# Tue, 02 May 2023 22:49:00 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0e57d29aa394d699aa77600e57970db6b5fd45693dfb1c54d1115b7e3878289b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63595273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4db6cd3459e2e072535da97940ce4b372a03da87ec094f467d388db12e0bb8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:48:42 GMT
ADD file:17739fc730ad8febc64f53eec61cbf10f8d2c5184cfda5466e89ab423a88f9d6 in / 
# Tue, 02 May 2023 23:48:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:56:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0b827c534260a55126ac3b18c14ea9160a3a3a03448b5c2b4462f9f3f4cf0ab`  
		Last Modified: Tue, 02 May 2023 23:53:05 GMT  
		Size: 45.0 MB (44988077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd17e95dbc3bb5a7cf7bdbee8d7899ed8d444893e1912f357d5842e974961ce7`  
		Last Modified: Wed, 03 May 2023 22:10:57 GMT  
		Size: 18.6 MB (18607196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7a222dd2442587c7f298bcfbdc7a7e3cb33680233226065062780c80a2e80c9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69385356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ce7043fa01b98a22beacb47c1d950007f9eea235c732ac3900e9e29e76e295`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:23:28 GMT
ADD file:cb107aa90220a9fc72fe1e3aa26878752691d6e9eb04696738920b5834c6d9e2 in / 
# Wed, 03 May 2023 00:23:29 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:24:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:77a3c1a83d83f65ef8fd579d19879f09a4018e384f42cfa55f82d426f32ff840`  
		Last Modified: Wed, 03 May 2023 00:27:15 GMT  
		Size: 49.3 MB (49345262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc449f3c80cded292a5c3da27ab253ce49a715e2cf061c906852d4c1361f3bf`  
		Last Modified: Wed, 03 May 2023 17:38:49 GMT  
		Size: 20.0 MB (20040094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f72e39e9afafc41a977fb5473bad8e76a43acf64b9dcdd36ae96da85ccc765d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71146724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62cbccaf672251a1aa2e7c87c942d765a916e6d131740bdef9b5dafaa52bee32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:01:59 GMT
ADD file:4abf127b0d4037b2d94457a8ef168165ed6946fec0635fdaa845ed4ee8f74681 in / 
# Wed, 03 May 2023 00:02:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:32:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:125509149936f5c9fc010cb99811f5cb23108af74e034fcf0903d3f2cc08d893`  
		Last Modified: Wed, 03 May 2023 00:06:56 GMT  
		Size: 50.3 MB (50321774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23628ffd3337a657bcf7bf912fd2ae65600ff79f16df8aa7bcf04bf06963c1c1`  
		Last Modified: Wed, 03 May 2023 22:38:39 GMT  
		Size: 20.8 MB (20824950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:962f5f9acfce523c495e3e0936d47a4a52fcea5c0c1f2c1a5c283a7682c0774f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68861644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae722f76b5252c15c6d078819ea0f9233460ff9ab107d32e7586d6c6250e3d5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:50:24 GMT
ADD file:3eff171361a4eb801d0fe38f81ca109a46285fd25a23f84aa338364d49c0591d in / 
# Tue, 02 May 2023 23:50:30 GMT
CMD ["bash"]
# Thu, 04 May 2023 01:15:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ad09064fad2597f74f486eca3ca74c1f51072bf61093439cd70c0d5735689aa`  
		Last Modified: Tue, 02 May 2023 23:58:51 GMT  
		Size: 49.3 MB (49301428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f246edce9c0b9683c9f5b08958e2cf2f6f000a6f32e10bcf66c1ea9b99805cbd`  
		Last Modified: Thu, 04 May 2023 01:29:06 GMT  
		Size: 19.6 MB (19560216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f2c45cd10a9f1d9283c07d7ed19a309fcf5dbc9f2b418840184f9368c1a161bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74891719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da614eb65cb7556a375715b68d678e997baf242c14778ee064ef77c416eebed2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:32:10 GMT
ADD file:c9bb656a5f751ff13849f6ca569f657cfc8dbe757b270dfa6e9fe2181e699494 in / 
# Wed, 03 May 2023 00:32:13 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:71d18ac463268aeb15f1776de10a379de577489dfb1022fc92adf6187695aeeb`  
		Last Modified: Wed, 03 May 2023 00:37:22 GMT  
		Size: 53.3 MB (53307234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0418f9e193f610de7186baec4f50ba3dfb4d394491ce54a0bbbf54eafb72013c`  
		Last Modified: Wed, 03 May 2023 23:38:43 GMT  
		Size: 21.6 MB (21584485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:5d88cbda24cb0506aa03a696689377f3feee5d90901a03ed6dc66400660bd599
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64166806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6dcb4ea3e9a5fba64f7b29967c857fbf7a4676075bf7258b32dff5f7fd571f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:29:17 GMT
ADD file:4e365b380d9cfb77573624c399d3376d19fa5c7028c44b681071b426fb1c6db0 in / 
# Tue, 02 May 2023 23:29:19 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:00b560a8a3ee42c2d5518b952b9a3b4607b68cd9d7d22c5b7a687f3ec6144150
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67414747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e445bc618e9cfa718d2e8d98817570f44ea813eab217cee6a47613cd95b8afd8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 03:42:08 GMT
ADD file:f714218b704bfe42a591f19c2fc0360b178732edfcd6b12687ea572c74b84171 in / 
# Wed, 03 May 2023 03:42:11 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:21:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9cad3c2eaf2133414000bf2d83ce6816eb4031d5b81288493af8102df33f2e4c`  
		Last Modified: Wed, 03 May 2023 03:45:13 GMT  
		Size: 47.7 MB (47675884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb874f6d93e1207d1df449384b5b4da9e636d2ddcd17695b1ccc4c35a4af54c`  
		Last Modified: Wed, 03 May 2023 22:32:39 GMT  
		Size: 19.7 MB (19738863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
