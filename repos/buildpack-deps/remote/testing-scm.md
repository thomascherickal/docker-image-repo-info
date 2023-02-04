## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:4fca1a2cf2f1382c95fcb879be1ad67e6f75c867d19466def3ae3975d847699d
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c662ffcb44c979007e7fb140b28a4cd74f883737a6089e78435d41a6d4bed227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133875690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d10eca82d1261fd1fed8f3543587b363635de612581dee7e1a88d430536f4d`
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
# Sat, 04 Feb 2023 07:20:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:4e5912b196c98527faa75de1f03b026f5c2740634e4a9498c536214352bbd910`  
		Last Modified: Sat, 04 Feb 2023 07:28:40 GMT  
		Size: 64.4 MB (64444820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:af1f951d89bc1809c89f82546324e0fa7c110534d66a75db441315f950a13dc4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129454629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84677951be649e10b671e7c2a61e94bb7ffae62e1f2dab2cb4bb81464f471b86`
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
# Sat, 04 Feb 2023 03:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b85ad8323370f7fbfbc955cee459d994385944146584314db17353d54e588b16`  
		Last Modified: Sat, 04 Feb 2023 03:22:13 GMT  
		Size: 62.0 MB (61978188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4bbb24bb0ecc806075782f2b5ae821d980aa471190364a6509e20f1f11b40ee3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124184637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1999988a5b1eed26396faa13d55808f3b3436ac68b20774c5995700191feb55`
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
# Sat, 04 Feb 2023 10:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a385e0a6d4d5d7a96989b13b2566ab1876cc3c1183e9bb336d6f3fbfee7df420`  
		Last Modified: Sat, 04 Feb 2023 10:58:19 GMT  
		Size: 59.6 MB (59629907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f99d3de7d1dade7396b45fa29fee449cf61e16dbc9bce5ebc3c4578f3b86b4b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133604253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c449e7578962ab3aa65e6262f0d95cf1a5f467d17f116a9c60be9d4b32e15d`
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
# Sat, 04 Feb 2023 06:43:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:e8f81f9fe3edb2827f590b523951ed4c6d26f17d9aa521c3b4da9f99c21d74bb`  
		Last Modified: Sat, 04 Feb 2023 06:51:25 GMT  
		Size: 64.3 MB (64337322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4b903beb883453ec5cc56f4c8709711ce5fe54092e1ea4da664b3ff103819bef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137178628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42bb74a0e693795d2afd68770eb2599fbbebe5ae6bdf64637f65e2174b4abf5e`
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
# Sat, 04 Feb 2023 08:17:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:4e9553d1e75be1e95f064cd22c826152b2da62a778c20ddc098b2c20f0575749`  
		Last Modified: Sat, 04 Feb 2023 08:26:15 GMT  
		Size: 66.3 MB (66316077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b97726d305cb7dd4287b949a409c1e516d5db47f13970c503f300dfea44e520c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129304267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:059c29a8d79cad005be487a4150a0dcbd37cf46a95116498fd105947dedbbd52`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 16:32:17 GMT
ADD file:aa37d39fc83f9cce3f1f8522cce22a9c3f9734fea6996431d00a2921079da343 in / 
# Wed, 11 Jan 2023 16:32:22 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:11:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:12:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 17:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:951f9db918ae0d2bc2c008522e4d5801e026653a12e21d76a02a48b96faaaabf`  
		Last Modified: Wed, 11 Jan 2023 16:41:22 GMT  
		Size: 50.1 MB (50120566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f5f91f049142f1806ecb72912bae28f718b88cdfc593aeaf7a39f089532f66`  
		Last Modified: Wed, 11 Jan 2023 17:39:47 GMT  
		Size: 8.4 MB (8398591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cee1eb44d9967c2535c5377493c304e9066c347f97119b605462ed59745bcfa`  
		Last Modified: Wed, 11 Jan 2023 17:39:47 GMT  
		Size: 11.1 MB (11104095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3efd79671fe172dfdbace9a335d8792f6cae970d99d15077cf26e204ebb898`  
		Last Modified: Wed, 11 Jan 2023 17:40:37 GMT  
		Size: 59.7 MB (59681015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cd4138795e144cae3c21791b02157f404c81f1a4c88e8b787bdbcba5214f87ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142185158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66dafc8aa33c01c6a9468dab84989afa2fd88ba26687448d67fe5723d8a92cef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:48:20 GMT
ADD file:be85aca9c16cf896fbced9508d29913a52fd69f8b2fd24c49efca520a37eeb1e in / 
# Wed, 11 Jan 2023 03:48:23 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:09:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:09:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 07:10:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:752672804a573b7cec5745cda59b6068007db5af1aef95a3e7929331c20247e1`  
		Last Modified: Wed, 11 Jan 2023 03:54:09 GMT  
		Size: 54.1 MB (54143855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750945def87bc453cd91c327bab81f39d93adb5ab86cdb4c913921aff512e2df`  
		Last Modified: Wed, 11 Jan 2023 07:24:14 GMT  
		Size: 9.6 MB (9612460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51845b4a51b4708da56bb53781c3d9bab20bd3820ac919ab7598b33948797a8`  
		Last Modified: Wed, 11 Jan 2023 07:24:14 GMT  
		Size: 12.1 MB (12114275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce18c9a581eda32c9677a56ce48754f33c6fce961d31ad0e8990173c2b6421`  
		Last Modified: Wed, 11 Jan 2023 07:24:42 GMT  
		Size: 66.3 MB (66314568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6d33f98b91d6f8cf77319662762b978aa54db9fd62025866077a4cd9a57ba959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130727553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e1e2f2ddbb74f3ed97c0e3a088b13a9072c67fa7d72367e8442184ca8623e1`
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
# Sat, 04 Feb 2023 04:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:50b390826d9588a3304d3449fb7e5d2594d77558be4387e3fb22b9188f1bc4c4`  
		Last Modified: Sat, 04 Feb 2023 04:39:04 GMT  
		Size: 63.4 MB (63413204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
