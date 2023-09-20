## `debian:stable-backports`

```console
$ docker pull debian@sha256:6cb29c6a7f9755669a55be9e80814ceffadc49576e429761acc768c0fca396db
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:ac790459e0ed53ca7bdb054d2b1fae28e4c95e2c1a9d6edf26133db21f7c9292
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49557400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368d56b3969cecc5f964eea81d55fdc695a834ef4110661e8bb3dabdf7123f21`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:22:44 GMT
ADD file:3b4850bdbeda4f6d961dfd39270718629c9294e17fb6544aa1d589e267c15598 in / 
# Thu, 07 Sep 2023 00:22:44 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:22:48 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6a1c5bff52cff72e59992ac0a97323470e2ba408b87d78984bd278e9cdfc4273`  
		Last Modified: Thu, 07 Sep 2023 00:29:04 GMT  
		Size: 49.6 MB (49557178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bcfa9b77e759a69099456101efbd22dcf23482204f13f600f465efcfbba955`  
		Last Modified: Thu, 07 Sep 2023 00:29:14 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:c1f07d71fbe30eee6f9815354f333faecebae2625087b17abf84f4381cea1265
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47415215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d52b1365c190c01e79023eaea411c355565736a77d1c53b6df7ae5bacc3534`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:51:25 GMT
ADD file:53ceb96e5672e219aca6daea64bd7cfac4dd9ef4811d93e8f1425341c0b5143c in / 
# Wed, 20 Sep 2023 00:51:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:51:31 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1360ba697847ba50544626e2fdf28d6189f0906348cc31ecb1f8ae807f15a790`  
		Last Modified: Wed, 20 Sep 2023 00:57:23 GMT  
		Size: 47.4 MB (47414993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82384d58a25e38f5b3c0107a834b251df6167c28353743617ced7d51385a58a6`  
		Last Modified: Wed, 20 Sep 2023 00:57:32 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b9cece93d0aeab6fc7177ca62c73b11fdd9a557b96237de5c3b10ff308f3d646
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45233453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c61b005a40bfe183974608ea9bfc7c0171155cde07c45d5b3995b930b431531e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:59:44 GMT
ADD file:de1cee8ae1fbc859725e0aee9a6c96b5319fc347f43f1a2c6d6f222639d7e022 in / 
# Thu, 07 Sep 2023 00:59:45 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:59:48 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2b21511435baa8f5c4133af9b49f91568e4bed6fc53b194df341e968994bfcb9`  
		Last Modified: Thu, 07 Sep 2023 01:05:48 GMT  
		Size: 45.2 MB (45233231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98df0876940f27bdb992bb68388dd121f9ebfce177774f6c1725b53ad639ba13`  
		Last Modified: Thu, 07 Sep 2023 01:05:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e00dfd4bc9a982a9d068e46752fa6badfac91e0c6a3c10c22ecbb6710137157c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49592067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f23ad459a1e7b4a6283836bc6f365927196217b89e5e58b465ad21ea0fdea22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:29 GMT
ADD file:ec644050dc5561e64384a4e0d183df970aaeac0750f1f762ffe29b7915295eeb in / 
# Wed, 20 Sep 2023 02:45:30 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:45:32 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d3dcf5c113a64725cb576d2f4e678aa926bd6ae3c3f413cd83e23503819fa61c`  
		Last Modified: Wed, 20 Sep 2023 02:50:30 GMT  
		Size: 49.6 MB (49591844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0945e730b58d50b3bf97b17885f7a47077182ab5cf6bfc4698ae0f3dbf1f3d73`  
		Last Modified: Wed, 20 Sep 2023 02:50:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:24347bd56442601a884eaf625cbdfe0fb4ca25e298ae4e0c776e395434f7766a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50569192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd2fc574aebdd8c4223b3ab84a09b64b3005ae3136a468e910d6cb8487f9eb0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:43:55 GMT
ADD file:a4f2fa3e98a8185764341fd63ac3591952b23182853ddd2ebf84ca98a3169ebf in / 
# Wed, 20 Sep 2023 00:43:56 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:43:58 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e4737eadb65c1f5f944f365a8626d47a469de86152a9f43f1178dd43ee1507fc`  
		Last Modified: Wed, 20 Sep 2023 00:50:38 GMT  
		Size: 50.6 MB (50568969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461c1d5dda8eb5ef020bf7a9130f1f9080afd3804c54012f114d2c13e5028390`  
		Last Modified: Wed, 20 Sep 2023 00:50:48 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:a3426cc4606e0219a3da4b99a404fb4922136e8db8cca8180a8787a1ae401626
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49542604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2c60764dd42ae95c06779e569a8a6758561da018746eec360c96f141e385de5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 03:14:12 GMT
ADD file:0f58f69aea93341db2a8b649d150e02eaa4a5504313cad47a7363c84670830a0 in / 
# Wed, 20 Sep 2023 03:14:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:14:32 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:54259548d3370f255becb131e7aa6e1bce367a442b76dc799daa0fa7ea1de9d5`  
		Last Modified: Wed, 20 Sep 2023 03:25:34 GMT  
		Size: 49.5 MB (49542379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c762ca16d6df56e4c27a9e3151d994b3a7b1f34ed12d3b9168812b9f3cf7943`  
		Last Modified: Wed, 20 Sep 2023 03:25:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:d42576ff152c81a37ccfdbbc4ddffeb7bfaac739004f3d99a73539102d7f85e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53542988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3cf09e1ccccc7cdadf5ff2213f6da461d73e9ef71d3be2f8953586334acf59`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:19:35 GMT
ADD file:98a533946d5ec81f51bed0170ddbc76778b25d23606300ef1b71439482282b88 in / 
# Thu, 07 Sep 2023 00:19:38 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:19:43 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c66f8f37cec4a11beaf7390ea808b815dc23493bee08237c260705d7f08bb452`  
		Last Modified: Thu, 07 Sep 2023 00:26:18 GMT  
		Size: 53.5 MB (53542765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155a4e8be8cbe542df6a13987febe75cd54b0524141836b517f6cbaed184295c`  
		Last Modified: Thu, 07 Sep 2023 00:26:28 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:01f4f6a3bb2cfb16ede3bee9d56b882dc827179c797f33fc18932253ef9737c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47921992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8945029783e1c3c586fbaf15ba0031c4ce00050a6e732300875ecfd8f3d66de5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:56:19 GMT
ADD file:fc6cba255c7e2ca2b3c811950c43cb205c3af8556fa9d269cc5d59271bc28bc5 in / 
# Wed, 20 Sep 2023 02:56:27 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:56:34 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9c4c8e345cd7d3d64eaa70c6bf00a5d3a9abe22d4184e1384d995a1d2ad16547`  
		Last Modified: Wed, 20 Sep 2023 03:01:25 GMT  
		Size: 47.9 MB (47921770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4b588b0f9f18a8d8fafaa0c7a42b46c78ada64f56718de994ca84886b98bb6`  
		Last Modified: Wed, 20 Sep 2023 03:01:31 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
