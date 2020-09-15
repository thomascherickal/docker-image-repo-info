## `debian:experimental-20200908`

```console
$ docker pull debian@sha256:a7988e105dae105d527cbdd570b3338997e6c666a376a047c4a2f4eb07b58cde
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

### `debian:experimental-20200908` - linux; amd64

```console
$ docker pull debian@sha256:d6a70214f3642773dd408084136c59dc30c696d1fbf99530e0a134447dd721c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52488330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc45c74be5094e4f5e37db4a2236ab4679944fe4e046ec36ee9b388b90117394`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:31:45 GMT
ADD file:29f2d9a3684156390fae91be6a412b3141b7afc9f93faaace93303249fbf29f6 in / 
# Thu, 10 Sep 2020 00:31:45 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:32:12 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:74323b006a6ff003707d36f504aad0df0c984b5f39eafee869c7cc79d74530d2`  
		Last Modified: Thu, 10 Sep 2020 00:38:32 GMT  
		Size: 52.5 MB (52488106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da14c71eec60270a33717071a5b1aa8ddcc5867bc66c61a0ddf905cc41e8bb`  
		Last Modified: Thu, 10 Sep 2020 00:38:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200908` - linux; arm variant v5

```console
$ docker pull debian@sha256:0c865b2e542f9e07d9779baa968d0406e6f7c6505aeb289b1fc6d7b4ef010fcf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50413737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:832d481c12ef3e1e09f1cd2553590016f31b89bc31bf1296beafcb3c29609cd0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:00:00 GMT
ADD file:e908218b894a70c32622fa9941322711662bd03c405cbeb25a1ca6884db90f96 in / 
# Thu, 10 Sep 2020 00:00:02 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:00:31 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6d19590209ad2cfa36a2a3b968d5c010ea5c44d2c0f7d24f68dc25a0e65181c0`  
		Last Modified: Thu, 10 Sep 2020 00:08:25 GMT  
		Size: 50.4 MB (50413513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f54081308a171f3cab3d028db5fd6cfaba99999b17b38d71d1b5545929f2702`  
		Last Modified: Thu, 10 Sep 2020 00:08:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200908` - linux; arm variant v7

```console
$ docker pull debian@sha256:d8762c19b82013cba9305702cc9aea1361788a3b48c1c41ad5b57d9f8722694c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48157028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e1852a630ca551f1c6ff46858dbde760595b5b5e3ea833171d38cca9ba0d10f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:15:14 GMT
ADD file:ba3a49a0dba0b04593fb9ed178da4b32bcb34d3bb852ef5c328492b1a272f166 in / 
# Thu, 10 Sep 2020 00:15:16 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:15:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:97bc442656068f8190a24c59bba055cb9e80d8df48c9fd447bc74f3bc9f26f90`  
		Last Modified: Thu, 10 Sep 2020 00:22:34 GMT  
		Size: 48.2 MB (48156803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc99baf12d89db8be45ed782344339fbd2513bbdd103c4e1344bbea18200f867`  
		Last Modified: Thu, 10 Sep 2020 00:22:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200908` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:0c7df49390d74a4bd0f593caa17392837d0efd56418e9ced9eb3eb1638fac64d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50845512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2275354af4be6957cb4edae09e5e4da86db103d6508492c55eac00e46a818e8f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:56:26 GMT
ADD file:98ab3713d41d2c9c5daef680b2b39489cbc0a6d092614b84e4895154494c09bb in / 
# Wed, 09 Sep 2020 23:56:29 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:57:06 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:03bc6921b1ca37f683765a6cfd3b562c4dfe7317d0653af5c635b37894cf5db6`  
		Last Modified: Thu, 10 Sep 2020 00:03:18 GMT  
		Size: 50.8 MB (50845287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e23fbaee62410e93618543bbab353a72e79d9d14e991b9ad7e53d06d1d45f9`  
		Last Modified: Thu, 10 Sep 2020 00:03:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200908` - linux; 386

```console
$ docker pull debian@sha256:acb1763d9c2b498bb4c56ab25d483cb5edd530aa1af9a46738c67fee28af9b0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53575213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5edc0d1562d1a01cc2bb963a056d8aea2668e62e94a670f1c9c90c971b17bf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:44:44 GMT
ADD file:a15d74ed082a5f9646b8cbc6713fa276509d7167184dffc07364150d96711a1b in / 
# Wed, 09 Sep 2020 23:44:44 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:45:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a4503e34a9d323271d71b6a9fc8a07c23db223a0f86339a64ef99eeb470bb8ea`  
		Last Modified: Wed, 09 Sep 2020 23:49:53 GMT  
		Size: 53.6 MB (53574993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547aeaa3f23c8506ea710c322b4d883bbc3152248af2411fe8befad9146d117f`  
		Last Modified: Wed, 09 Sep 2020 23:50:08 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200908` - linux; mips64le

```console
$ docker pull debian@sha256:9b1060abad96e5a841dfd33dfff6a2be2cb1bcf0ce91a9db89d75ca21f818f00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51211393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9cbc031045b59dc8020ef69248f0c8ba4c2d6a10cdaa6bd768f2c3ef6fcd5c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Sep 2020 01:09:48 GMT
ADD file:6cf1f9f1fb0295ee5ac10ac35602f5a9b7b363d2264d568d6403e266857f405d in / 
# Tue, 15 Sep 2020 01:09:49 GMT
CMD ["bash"]
# Tue, 15 Sep 2020 01:10:12 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:83f49c9a27a5f9fa3f29bd73509d8c95522c362b6e8d815ab3abbacf9808c7ac`  
		Last Modified: Tue, 15 Sep 2020 01:18:02 GMT  
		Size: 51.2 MB (51211170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a38254243ea6b1a01baa4f06565fccda3cf3798ae4f5bf4669bff7e042c984`  
		Last Modified: Tue, 15 Sep 2020 01:18:44 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200908` - linux; ppc64le

```console
$ docker pull debian@sha256:ed7e418de6b60b4a8ceb4b2eefc5e05d527d7f26849010a5fb708078a7810772
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.3 MB (56336903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cba657dd7e59ba33461641b699aa50479d108bb51d9e44bb26d0eabedfc08ab`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 01:17:21 GMT
ADD file:fd34afd255174b31d6dd00ea6c9d86f639a66d0c08efbeb5b2ed479f3f854abc in / 
# Thu, 10 Sep 2020 01:17:34 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:20:52 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f6ce093fdf958f0defc21bbd6b342928a0ebea1b7187ebd43183fbc574a4e5b8`  
		Last Modified: Thu, 10 Sep 2020 01:40:43 GMT  
		Size: 56.3 MB (56336677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c269067e32de3313b0cd97f9136947817a964aa1bdc440f52d7a2891dbaabe93`  
		Last Modified: Thu, 10 Sep 2020 01:42:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200908` - linux; s390x

```console
$ docker pull debian@sha256:be10aadd6b1df9f5ed28e8d27fc68a5a275865ef2c4c1beaa61340d270e74b57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51061252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6082bcd64f693d115af9c6f15732f2cf531e385ea8b96fb2a6af35ca9e781608`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:44:45 GMT
ADD file:47122f980693a5efb3b9803fdc722b3f977308b1a7c3f97576bf28650fd88544 in / 
# Wed, 09 Sep 2020 23:44:48 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:45:14 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2f2fd18bf6b5fe6e3937dfb58f9297c8502c3e601f2debc1cb4869e1f360f871`  
		Last Modified: Wed, 09 Sep 2020 23:47:54 GMT  
		Size: 51.1 MB (51061031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf4ecc6617f4dfbf910394c28eafe378845e004bdae992017166b968b92ee7`  
		Last Modified: Wed, 09 Sep 2020 23:48:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
