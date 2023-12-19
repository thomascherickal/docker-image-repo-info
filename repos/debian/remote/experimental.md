## `debian:experimental`

```console
$ docker pull debian@sha256:9498694dbad50918e866f3e21e1cd8df24ec8ac67f38b91d9bd914fcd27d816c
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

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:c3c489139dfbf095085247562b0a17cba9656eb395dd86821485bab3578aec87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52247047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c9ba25194d4f03f0a863126acc26fc25cf914cdbac0d902649a290fc205dbd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:23:30 GMT
ADD file:a15103578eec126916f03fcffc30fc68c2784ff4137ab891659c15c648ae0458 in / 
# Tue, 19 Dec 2023 01:23:30 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:23:44 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ac1e917d2652641c1443e5c509c042b31a6e06c85f5a4d97796b4212c9cd049e`  
		Last Modified: Tue, 19 Dec 2023 01:30:10 GMT  
		Size: 52.2 MB (52246825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc5401ae9c8d8003f3e684b1437f469200194a438d4b2271833468448bc8bd4`  
		Last Modified: Tue, 19 Dec 2023 01:30:32 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:707cf00330e59ce5e1cb9acd55078800b6014af51fbda859bd43486532d073fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47266286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:197c2e61f19d5b57c017a3ada9900a15f8a4ab511cbe61f9a776e8edb5718fda`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:57:05 GMT
ADD file:1ad4ce430c88442f1130f70b99ac8bb1c7b6ca2b6e72cbaa4d28e1387cd20864 in / 
# Tue, 19 Dec 2023 01:57:06 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:57:14 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0a7a3869a18520688e4e53f422d45f34a4c34a812d80cdc1e982179484d53019`  
		Last Modified: Tue, 19 Dec 2023 02:02:44 GMT  
		Size: 47.3 MB (47266066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fee0673b2e926a8083b537be16cd967213522133c50c2048008e3c4b0af0254`  
		Last Modified: Tue, 19 Dec 2023 02:03:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:1398349d9be9f6ca48735cf55160d4095619bb7ef2936176135ea50bd96ed0ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44898984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc49f2727aae1d8ba1209b179803ed8631d7757a97180f9f12b2f01d848e825b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:10:22 GMT
ADD file:8c572d76514c8c3ab2fbc43b33253870636fdd9346ec932b8b28fb144417b995 in / 
# Tue, 19 Dec 2023 02:10:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:10:33 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ef74c9caa47d85169a03d60e3f17305d9a3aa24a2699bf19e2c9a7231abb198d`  
		Last Modified: Tue, 19 Dec 2023 02:16:38 GMT  
		Size: 44.9 MB (44898765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394aa29505df7884ab0b087fd74b8f1f2322e22f678e6cfb08cdbd0e8252c6c`  
		Last Modified: Tue, 19 Dec 2023 02:16:58 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7ac54b683197b79aaadca21cccd9b4d99c008ac83332e2701571216306bbc383
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49690032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f395af462003e1e25af91cd8d9cb504b81f3c270a4ec07186bdb125df022f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:43:09 GMT
ADD file:ba5dd365f875207e1dd5cf456a6700fba8d9523bdcccadb14783bcd1ebdc1a8c in / 
# Tue, 19 Dec 2023 01:43:10 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:43:18 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2aab20151d2b9073aa22f609ec58666e04cbdaba4d6482dfc7b6cbbded98d393`  
		Last Modified: Tue, 19 Dec 2023 01:49:23 GMT  
		Size: 49.7 MB (49689810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23778b90b7e9176dcefef10573d5c79fb7fe3212c92d0cdea26a09225cf9ea60`  
		Last Modified: Tue, 19 Dec 2023 01:49:42 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:b282ca696fad9a440c7f53da0b166ddfc4ff176022ea89bee6fa59431fd05f1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50559480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00dc49934329a988456e0f9b19a1ca6ed44c6ea9ad48c1b3039889e7011136b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:12 GMT
ADD file:c306ca084269bac3e73eca11b9cf1fde32b2438ef4a2daf50aa7d796a583b727 in / 
# Tue, 19 Dec 2023 01:42:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:42:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b251e852034d95763dad2b2bd66c9c9046c09adac90fa5b77002410e77e32ca3`  
		Last Modified: Tue, 19 Dec 2023 01:49:32 GMT  
		Size: 50.6 MB (50559261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83592bf926afec21b96646cdbdda37310bdc738d957dc6b99bd14e41f4d63c86`  
		Last Modified: Tue, 19 Dec 2023 01:50:01 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:0c7e43fb354df78f6ddb66e620f331543698ed17ad9e8a4f636e7f1389469ae0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49348069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d296171bec472fbd0e31f81c100b2330f3bfacee28a8aab8b5a56242b52c55`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:21:33 GMT
ADD file:84a1f7155d4dfd433fef3204de38861d231cda5320de89584741b14da1e4c1a6 in / 
# Tue, 19 Dec 2023 02:21:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:22:21 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4fd948dbc4658e150756cf1c458b5d880c3b99ae83cf2208a9ce82b46b1f3dc3`  
		Last Modified: Tue, 19 Dec 2023 02:32:56 GMT  
		Size: 49.3 MB (49347845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a91429edfd93e0903aca100a9e8bfc6a257289ff5655cc3431d3f897364b730`  
		Last Modified: Tue, 19 Dec 2023 02:33:35 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:363296841e6bbbcf0f0f360d0e5975cf3d4de993e576d6084aa7812e1f58902a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53455919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de49033379b62fc7d8367d1d79ed602e018b3ff36cec525d55e10fec5e1314a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:24:40 GMT
ADD file:0af0381b54263356d67da658e91aa4daf9a7626ec1eb50937a01f950c70269ae in / 
# Tue, 19 Dec 2023 01:24:43 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:24:57 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bbd2991f9801d49e2e978fc288252c5eb7d6e502ce66c9ba0d1bec7394a94f99`  
		Last Modified: Tue, 19 Dec 2023 01:30:50 GMT  
		Size: 53.5 MB (53455698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b07a8dd4ef570b865cb61683551cacc9daff3728e5e2f63ccc1a7cad5fb942`  
		Last Modified: Tue, 19 Dec 2023 01:31:14 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:e0bf38cfc5462b792b87e71081f3ae37d56da48a46f61a1446b03c1a65cdbbbf
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48232774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9dadeb4e9e455ad05c8f8a61ace661f7863bb03519ce93058c91748067cd94`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:11:00 GMT
ADD file:cacd9b8eda0a4db6199752d3c802d84baa80f1cfb12c41e0c567aea97d7d6f76 in / 
# Tue, 19 Dec 2023 02:11:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:11:36 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:63f5282077c764e50b037060efc122153a325e5126b84d94374504cf95b4b665`  
		Last Modified: Tue, 19 Dec 2023 02:14:11 GMT  
		Size: 48.2 MB (48232549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b94132f8863bc3e6ceee88d025f4ec9794193b63d54500eec256ca40fef10d`  
		Last Modified: Tue, 19 Dec 2023 02:14:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:43a5891c839c84d8f00810d182dc7deedb90f7501e016622111a2e517e4f59b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49328408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2197ae7fd96dd8061f82064e02169216990665b0b1692c7e6a5cca87df3db77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:46:00 GMT
ADD file:eb03e79389a9a1f4792c7626177965861c32abc4748916db20ba724280d5f823 in / 
# Tue, 19 Dec 2023 01:46:04 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:46:22 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b28c9c2dc4e251d259f8365924ee2d21e2009c71547be061b371715dc3b1a975`  
		Last Modified: Tue, 19 Dec 2023 01:50:24 GMT  
		Size: 49.3 MB (49328190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929b7667049be57c42cf6e22296c8733c1f0232829d20ef83ab5fa4f6e9b037a`  
		Last Modified: Tue, 19 Dec 2023 01:50:38 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
