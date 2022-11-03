<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fedora`

-	[`fedora:35`](#fedora35)
-	[`fedora:36`](#fedora36)
-	[`fedora:37`](#fedora37)
-	[`fedora:38`](#fedora38)
-	[`fedora:latest`](#fedoralatest)
-	[`fedora:rawhide`](#fedorarawhide)

## `fedora:35`

```console
$ docker pull fedora@sha256:545ce1f4502d6fa7774d647cff7d48587a57ed7be5dc5eb8442fc6333f94c1be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:35` - linux; amd64

```console
$ docker pull fedora@sha256:8e5852e0a72101197de788437844ae9e1b382b719ba7ac7cf482804e0ffa04f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55740531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d0cdfd5d956c392500708fbb1c82aa81a5e51c75c68448bd411ece20cde2f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 01 Oct 2021 23:02:34 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Thu, 03 Nov 2022 20:40:27 GMT
ADD file:f696eb87c7de0bd8a2b1679c7d4cb0e3a0b284278592e1e6082b16368b1b02fe in / 
# Thu, 03 Nov 2022 20:40:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6153fc78ad283cb10dc19fe1a49cc6c088872832764bb163196041ea3cde666e`  
		Last Modified: Thu, 03 Nov 2022 20:41:31 GMT  
		Size: 55.7 MB (55740531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:35` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:fc7ee019f1977a7b70a7d99788404371e544c09e4fa37982b49a14afe2bfa264
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54707201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030df6379def1dccab6fc02b9ffcfada2488e548fda849c806782d05d486ac28`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:13 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Thu, 03 Nov 2022 19:58:16 GMT
ADD file:08864f699fa316c00a84bd5ba7b5db70ec8e27c8c9fc8d882dd1a4689189ceaa in / 
# Thu, 03 Nov 2022 19:58:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8a3ce182e3ca69fe49d239073d8adfc5689c182afd5a08168f296b3837429577`  
		Last Modified: Thu, 03 Nov 2022 19:59:04 GMT  
		Size: 54.7 MB (54707201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:35` - linux; ppc64le

```console
$ docker pull fedora@sha256:60b722cb640221e50943c5a8801099ba61004ffe36f1dbc5a3c52225acfb6327
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.7 MB (60682412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4cae0f2e6393f816b38b6c0acc95a5b58bd27cda534bdc485870b9ce72b705c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 11 Oct 2022 12:17:07 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Thu, 03 Nov 2022 21:17:57 GMT
ADD file:9b16c5218009e478c7b88b71868237f62ab6e258533618f342b85dd58206347b in / 
# Thu, 03 Nov 2022 21:17:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ab5754c22ec4f84a6ecabe786e2bd2a40b91174d8b871fd5ab885ff6132f00e0`  
		Last Modified: Thu, 03 Nov 2022 21:19:57 GMT  
		Size: 60.7 MB (60682412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:35` - linux; s390x

```console
$ docker pull fedora@sha256:eaece17de7169ad6c330cffd25aed8ab39fb4c029d2ba51f56bfc24e2667669b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53712303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f44304080a1001be431f1d634123d3515016652aa3e21dd95afd9e8d783c066`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Fri, 01 Oct 2021 22:42:23 GMT
ENV DISTTAG=f35container FGC=f35 FBR=f35
# Thu, 03 Nov 2022 21:29:31 GMT
ADD file:ea1ac8675d77c4ed9ed44b5ac4ad8d27852b387d1f367820c7b277d43c5459e7 in / 
# Thu, 03 Nov 2022 21:29:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1050d8d66c26d92c5f344f5f7533fc09ca8958a1a6ebfa55c7890bf737486a7c`  
		Last Modified: Thu, 03 Nov 2022 21:32:16 GMT  
		Size: 53.7 MB (53712303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:36`

```console
$ docker pull fedora@sha256:d2c7dadebf6d8eb44ae87955cd02e1bc89fa6f9afb7452467a5524a8c72c208e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:36` - linux; amd64

```console
$ docker pull fedora@sha256:455fec9590de794fbc21f61dbc7e90bf9918b58492d2a03fa269c09db47b43f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (59995747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7654d129a8a25626dce55adfa5d8a419b794952229ed9542968ef7faca2ee975`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:00 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 20:40:40 GMT
ADD file:8d61743db71ec38169aae6644f4ef369766e0bece381549d7530d11df9a9a214 in / 
# Thu, 03 Nov 2022 20:40:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e437052d4f94147f80c5b03d10b6d7e034a32b1db5a9f340b2c8090cec1376f8`  
		Last Modified: Thu, 03 Nov 2022 20:41:48 GMT  
		Size: 60.0 MB (59995747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:36` - linux; arm variant v7

```console
$ docker pull fedora@sha256:ce3d46c564d9145f73d1618a605e9d959ec704d409b2afb54f3517a27c818cc6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54490837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d6e76519a089477b47efb6d84e8dcbc6639cc6a12e03d575b069278e4cffa88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 20:46:50 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 20:46:50 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 20:46:56 GMT
ADD file:2a100119d250f9a75cfee4425142172c6ec02864e33737f0dd9e8330ccecce4a in / 
# Thu, 03 Nov 2022 20:46:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:af068febaa0f76501a770f13db16f57d1900b8d9c746a4ec074e4c234de151b5`  
		Last Modified: Thu, 03 Nov 2022 20:47:22 GMT  
		Size: 54.5 MB (54490837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:36` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:e25982afd0124a42b8fc8029b31919f5e349e5ef6e75e7c51f5ad6175c931890
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58073695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade8b003ba4713a478328aa7c17d60571cebd32d3b49494ba316ae1696443854`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:22 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 19:58:26 GMT
ADD file:b82910bf07012170f0d5f59e76752b39c1697ba5f4f170c1e130973bb3cfd444 in / 
# Thu, 03 Nov 2022 19:58:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:abb467b93dbf4d81a9c5342c20b37ddd6b97aac043b7d58e7add918604ce9bb4`  
		Last Modified: Thu, 03 Nov 2022 19:59:18 GMT  
		Size: 58.1 MB (58073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:36` - linux; ppc64le

```console
$ docker pull fedora@sha256:72ed15e0fd3d47ae2f15282121a16a70e1e160450dd7a5c18f929904e86dff16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65410552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e5939540b7d8a7c6688a99727185fdba334c9badb2ebd87277fdba08e936e2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 11 Oct 2022 12:17:27 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 21:18:22 GMT
ADD file:1d9d84b7845e61a4beda77c6785383e27562f7e2fb2bcfb54ccd4138b2730c3c in / 
# Thu, 03 Nov 2022 21:18:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ad8408f5b2d2dd65fa3ca093ea3b2dbbb1e17e0320fb0d56ae86c11352f276a`  
		Last Modified: Thu, 03 Nov 2022 21:20:23 GMT  
		Size: 65.4 MB (65410552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:36` - linux; s390x

```console
$ docker pull fedora@sha256:0d627899e2c6667043adba2a4e7468fc28cf2ab290dbfb61abce7acbb9a70bdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (56970167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89673282ade36f6e3124b3e042ea2aa09075705ba6a816f186b5bc6c4127528`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 04:31:33 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 21:30:11 GMT
ADD file:2d9503540999d2f7035cfd3b17a8bbbcc9cc55cb4fc9218da2cf0ce74850c6a9 in / 
# Thu, 03 Nov 2022 21:30:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:49b3b9a3bbb38db44811f93b55b63a5d766ced4b6f0e968ca2279cf9a430db27`  
		Last Modified: Thu, 03 Nov 2022 21:32:31 GMT  
		Size: 57.0 MB (56970167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:37`

```console
$ docker pull fedora@sha256:47e02427fb5d8161a8e6f63428ed848073c67bed84f903e71fbdc9dfd61e0884
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:37` - linux; amd64

```console
$ docker pull fedora@sha256:6184fcbfc8f27fda21d0f7a69c74b0f7bcd1a61ac9b566b8d6a3a3adefad1657
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65990425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b88d41f1c8cc270ffcb792f1e914928c148f8f0620ca5de6e384767e57369e6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:14 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Thu, 03 Nov 2022 20:40:54 GMT
ADD file:0226ce47da6a83519e0692ec1a9c5b587dc79a25d69ebeeaedc3780074f29d21 in / 
# Thu, 03 Nov 2022 20:40:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0798f1d8aae23f95c245d28fd50b7c68bee321534c9809612e323eb988c2b3a4`  
		Last Modified: Thu, 03 Nov 2022 20:42:08 GMT  
		Size: 66.0 MB (65990425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:37` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:0426ee652c0c3bb9531d1b39ad754bd67ae822d9ca16b676380a92b309604c3d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64205162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4aee74be4b697faf1cda9c87e0bbf70c6f527fa25134db996767711b1304fbe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:31 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Thu, 03 Nov 2022 19:58:35 GMT
ADD file:3a61d7bdacda5462a48fadf1ec31cd50495224f98fe81e79d45516f0a00e3484 in / 
# Thu, 03 Nov 2022 19:58:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8a2030335a3fd921272d37d29cc9b1ecbd412e2223ad79a42c8acb126dc554f4`  
		Last Modified: Thu, 03 Nov 2022 19:59:37 GMT  
		Size: 64.2 MB (64205162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:37` - linux; ppc64le

```console
$ docker pull fedora@sha256:f54ba1eacd025e9fe50e8ccb92dd9fa106f3468f283655894bc68c434e97966d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71682863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8d3c9f069634c4cee7af46a23ac3a873bb598cb7c4c2f17832068612c5f1ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 11 Oct 2022 12:17:51 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Thu, 03 Nov 2022 21:18:47 GMT
ADD file:bba6b2c837ef0a16d2b77ae80936001432060d29808972351ac2a64147c6489c in / 
# Thu, 03 Nov 2022 21:18:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8e1b4c7dc67dab15b509d7f6703cfd23a62d9288837a87c02bcbfd115011ece7`  
		Last Modified: Thu, 03 Nov 2022 21:20:55 GMT  
		Size: 71.7 MB (71682863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:37` - linux; s390x

```console
$ docker pull fedora@sha256:77e2f2cee77d1f7197690ead050f69f6e9c11e3743a4e8effb85386168b1de79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63144081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d04736ab24260c554e90c9726864eeec46b72a99b53cb7c451822d1e026c84`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 04:31:50 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Thu, 03 Nov 2022 21:30:49 GMT
ADD file:587c1fe8d0e2bd058b29c3bf96526419c2686f790b04383f23a3cb4320289346 in / 
# Thu, 03 Nov 2022 21:30:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d312ec80b6aedcc0a698102bc74e93710ec85c2591fb356555acff0e92d3c29a`  
		Last Modified: Thu, 03 Nov 2022 21:32:50 GMT  
		Size: 63.1 MB (63144081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:38`

```console
$ docker pull fedora@sha256:6815faf4fa28be5236e05e319d5af35afc721c698566cd9fe37b6014018190fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:38` - linux; amd64

```console
$ docker pull fedora@sha256:c7dfa518d9db440fb02362c0f9b014c0e1b8e04bc0f6bf540d1d5ac2ecb43453
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65568074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b902325de1ec96bbbeecd610ef5dcfba06da72e6831eb0ac1049e376d7778a58`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 20:41:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 03 Nov 2022 20:41:08 GMT
ADD file:aea454c4f9f7bccbd03cf61c6477deac629e6b63f8ef39d87667ee4efaf12136 in / 
# Thu, 03 Nov 2022 20:41:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7658a6d4e9efd0ec04b7aca3c754f4441c79d4dedab19a67c5f5293bb0b5e151`  
		Last Modified: Thu, 03 Nov 2022 20:42:25 GMT  
		Size: 65.6 MB (65568074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:38` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:b4fc674566ca392e7117508f46519362a53f2c32147cbe8ae6e59a7ebe8b93be
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (64007024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24e8e907dcbcc2c2b343c0c9bc5281dbccea310bcd3a98d2d7037e39f3929705`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:41 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 03 Nov 2022 19:58:44 GMT
ADD file:d63621367aab7d458af7e75ba42437bc50c5c9166122e52b7a46c5cea2e22147 in / 
# Thu, 03 Nov 2022 19:58:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5acecd05a9bc955b7cb9f11323f55414ce45efebe26d8fd51c2f920bdafa3c2b`  
		Last Modified: Thu, 03 Nov 2022 19:59:52 GMT  
		Size: 64.0 MB (64007024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:38` - linux; ppc64le

```console
$ docker pull fedora@sha256:bbc10a3fd25705b990ffa3c3fefa49911129c29763a9a66c301bf30a927e3afa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71231033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b6a61a694cd3ae5798c3ca7b97f8278e0dc054bbd5b8fd1e33d33e3cdf767b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:19:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 03 Nov 2022 21:19:13 GMT
ADD file:c5bf5b641727fb8e7c31aa41672e0ddb05df5c6eaf89a0f843077ca40a47fc7c in / 
# Thu, 03 Nov 2022 21:19:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dd28bd1e5a238b01fff9e8ef41017687d39ab4bc32b334d1e20bd91365c70797`  
		Last Modified: Thu, 03 Nov 2022 21:21:22 GMT  
		Size: 71.2 MB (71231033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:38` - linux; s390x

```console
$ docker pull fedora@sha256:3b4472d794cbba47ecb920cd22eaf9cfd309e9a8cf8c032c90c1f9f29de28861
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63138998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301cc64c2ae848873eee3f049c983d01a499bb1f15eab17cd1bc6e5785d05bd6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:31:13 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 03 Nov 2022 21:31:29 GMT
ADD file:27e61c1774070ba18a01440dbe07f7b3515255904927dc4486d2910ed6c1ce53 in / 
# Thu, 03 Nov 2022 21:31:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6164846894a3e2ee22b7f8e889b9070fcbdc89fc1b4c53e365e3229dd9e0759b`  
		Last Modified: Thu, 03 Nov 2022 21:33:04 GMT  
		Size: 63.1 MB (63138998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:latest`

```console
$ docker pull fedora@sha256:d2c7dadebf6d8eb44ae87955cd02e1bc89fa6f9afb7452467a5524a8c72c208e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:latest` - linux; amd64

```console
$ docker pull fedora@sha256:455fec9590de794fbc21f61dbc7e90bf9918b58492d2a03fa269c09db47b43f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (59995747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7654d129a8a25626dce55adfa5d8a419b794952229ed9542968ef7faca2ee975`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:00 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 20:40:40 GMT
ADD file:8d61743db71ec38169aae6644f4ef369766e0bece381549d7530d11df9a9a214 in / 
# Thu, 03 Nov 2022 20:40:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e437052d4f94147f80c5b03d10b6d7e034a32b1db5a9f340b2c8090cec1376f8`  
		Last Modified: Thu, 03 Nov 2022 20:41:48 GMT  
		Size: 60.0 MB (59995747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm variant v7

```console
$ docker pull fedora@sha256:ce3d46c564d9145f73d1618a605e9d959ec704d409b2afb54f3517a27c818cc6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54490837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d6e76519a089477b47efb6d84e8dcbc6639cc6a12e03d575b069278e4cffa88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 20:46:50 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 20:46:50 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 20:46:56 GMT
ADD file:2a100119d250f9a75cfee4425142172c6ec02864e33737f0dd9e8330ccecce4a in / 
# Thu, 03 Nov 2022 20:46:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:af068febaa0f76501a770f13db16f57d1900b8d9c746a4ec074e4c234de151b5`  
		Last Modified: Thu, 03 Nov 2022 20:47:22 GMT  
		Size: 54.5 MB (54490837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:e25982afd0124a42b8fc8029b31919f5e349e5ef6e75e7c51f5ad6175c931890
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58073695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade8b003ba4713a478328aa7c17d60571cebd32d3b49494ba316ae1696443854`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:22 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 19:58:26 GMT
ADD file:b82910bf07012170f0d5f59e76752b39c1697ba5f4f170c1e130973bb3cfd444 in / 
# Thu, 03 Nov 2022 19:58:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:abb467b93dbf4d81a9c5342c20b37ddd6b97aac043b7d58e7add918604ce9bb4`  
		Last Modified: Thu, 03 Nov 2022 19:59:18 GMT  
		Size: 58.1 MB (58073695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; ppc64le

```console
$ docker pull fedora@sha256:72ed15e0fd3d47ae2f15282121a16a70e1e160450dd7a5c18f929904e86dff16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65410552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e5939540b7d8a7c6688a99727185fdba334c9badb2ebd87277fdba08e936e2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 11 Oct 2022 12:17:27 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 21:18:22 GMT
ADD file:1d9d84b7845e61a4beda77c6785383e27562f7e2fb2bcfb54ccd4138b2730c3c in / 
# Thu, 03 Nov 2022 21:18:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ad8408f5b2d2dd65fa3ca093ea3b2dbbb1e17e0320fb0d56ae86c11352f276a`  
		Last Modified: Thu, 03 Nov 2022 21:20:23 GMT  
		Size: 65.4 MB (65410552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; s390x

```console
$ docker pull fedora@sha256:0d627899e2c6667043adba2a4e7468fc28cf2ab290dbfb61abce7acbb9a70bdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (56970167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89673282ade36f6e3124b3e042ea2aa09075705ba6a816f186b5bc6c4127528`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 04:31:33 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Thu, 03 Nov 2022 21:30:11 GMT
ADD file:2d9503540999d2f7035cfd3b17a8bbbcc9cc55cb4fc9218da2cf0ce74850c6a9 in / 
# Thu, 03 Nov 2022 21:30:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:49b3b9a3bbb38db44811f93b55b63a5d766ced4b6f0e968ca2279cf9a430db27`  
		Last Modified: Thu, 03 Nov 2022 21:32:31 GMT  
		Size: 57.0 MB (56970167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:rawhide`

```console
$ docker pull fedora@sha256:6815faf4fa28be5236e05e319d5af35afc721c698566cd9fe37b6014018190fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:c7dfa518d9db440fb02362c0f9b014c0e1b8e04bc0f6bf540d1d5ac2ecb43453
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65568074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b902325de1ec96bbbeecd610ef5dcfba06da72e6831eb0ac1049e376d7778a58`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 20:41:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 03 Nov 2022 20:41:08 GMT
ADD file:aea454c4f9f7bccbd03cf61c6477deac629e6b63f8ef39d87667ee4efaf12136 in / 
# Thu, 03 Nov 2022 20:41:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7658a6d4e9efd0ec04b7aca3c754f4441c79d4dedab19a67c5f5293bb0b5e151`  
		Last Modified: Thu, 03 Nov 2022 20:42:25 GMT  
		Size: 65.6 MB (65568074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:b4fc674566ca392e7117508f46519362a53f2c32147cbe8ae6e59a7ebe8b93be
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (64007024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24e8e907dcbcc2c2b343c0c9bc5281dbccea310bcd3a98d2d7037e39f3929705`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:41 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 03 Nov 2022 19:58:44 GMT
ADD file:d63621367aab7d458af7e75ba42437bc50c5c9166122e52b7a46c5cea2e22147 in / 
# Thu, 03 Nov 2022 19:58:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5acecd05a9bc955b7cb9f11323f55414ce45efebe26d8fd51c2f920bdafa3c2b`  
		Last Modified: Thu, 03 Nov 2022 19:59:52 GMT  
		Size: 64.0 MB (64007024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; ppc64le

```console
$ docker pull fedora@sha256:bbc10a3fd25705b990ffa3c3fefa49911129c29763a9a66c301bf30a927e3afa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.2 MB (71231033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b6a61a694cd3ae5798c3ca7b97f8278e0dc054bbd5b8fd1e33d33e3cdf767b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:19:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 03 Nov 2022 21:19:13 GMT
ADD file:c5bf5b641727fb8e7c31aa41672e0ddb05df5c6eaf89a0f843077ca40a47fc7c in / 
# Thu, 03 Nov 2022 21:19:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:dd28bd1e5a238b01fff9e8ef41017687d39ab4bc32b334d1e20bd91365c70797`  
		Last Modified: Thu, 03 Nov 2022 21:21:22 GMT  
		Size: 71.2 MB (71231033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; s390x

```console
$ docker pull fedora@sha256:3b4472d794cbba47ecb920cd22eaf9cfd309e9a8cf8c032c90c1f9f29de28861
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63138998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301cc64c2ae848873eee3f049c983d01a499bb1f15eab17cd1bc6e5785d05bd6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:31:13 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Thu, 03 Nov 2022 21:31:29 GMT
ADD file:27e61c1774070ba18a01440dbe07f7b3515255904927dc4486d2910ed6c1ce53 in / 
# Thu, 03 Nov 2022 21:31:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6164846894a3e2ee22b7f8e889b9070fcbdc89fc1b4c53e365e3229dd9e0759b`  
		Last Modified: Thu, 03 Nov 2022 21:33:04 GMT  
		Size: 63.1 MB (63138998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
