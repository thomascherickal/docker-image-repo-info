## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:5a5019125700d915a2909fbabc315cf4ea5d855054a98229ff7e231a2ed06894
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
$ docker pull buildpack-deps@sha256:55d3c9a086b1f3e2bf2efc43a3facd9259debb301bc36d744d399b9f9183baab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73888718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ca5ff02ac501d48c546df140a835f2ebdb2306a1a564dd635fc72f385dd9659`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:27 GMT
ADD file:69815228666696b3cd3b2799492e3d9cdf4f513ccca5c1cc9282f6c569cc8730 in / 
# Wed, 01 Nov 2023 00:22:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bf371b8152e5df155015cbda7e76bcf445a8be262f7017a9c2cd27a64c3bd875`  
		Last Modified: Wed, 01 Nov 2023 00:28:24 GMT  
		Size: 49.5 MB (49534303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdee5573ddff91e45c81d11193d3d33f964fe89aa56549950a84c64303f6c2f`  
		Last Modified: Wed, 01 Nov 2023 01:05:03 GMT  
		Size: 24.4 MB (24354415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2facb29855ce778449935650ad0bf8f05285f5bc037e27c0abc545731ade43e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70157877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3ce55c97d64bebc6d52e5b52a1e5ec90df23921d54256da45d2978fabdcf44`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:22 GMT
ADD file:32bc859b55e9b4aada411b379418b1cd95da1e1f72e89ade7698d0132f8edafd in / 
# Wed, 11 Oct 2023 17:38:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f4ea7fe7b8690c3ca25a1b3c670c2f82209d55ff6d955af872eb0ab8df5ff97`  
		Last Modified: Wed, 11 Oct 2023 17:42:28 GMT  
		Size: 47.2 MB (47164847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f544479290fab5feada5ea10b06b543b11d0716abc190b0d608b218fa5128b85`  
		Last Modified: Wed, 11 Oct 2023 18:16:56 GMT  
		Size: 23.0 MB (22993030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2a3ac98b13e5c0b84e8a96c479d489b7281c2542c75032fdcd02dda6af1de78e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67168379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21e5bc073011f98455f4bb3cf2cf376f08857422f623a0610bbb271406d9f9c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:32 GMT
ADD file:e83473ecad5aa9a153d02c535c6e40e22679b973268fdd74a0f5bd86b004222a in / 
# Wed, 11 Oct 2023 17:43:33 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:50:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b724b570b5800a7c354a5dac64a4fa673c71f6df8cbf449ab4ce5efd684dd911`  
		Last Modified: Wed, 11 Oct 2023 17:49:18 GMT  
		Size: 45.0 MB (44953579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525e6d91de2d1165a43ec12ba22c9f291c7d260542aec1bb8f5ffe58d6dd1c6`  
		Last Modified: Thu, 12 Oct 2023 03:59:24 GMT  
		Size: 22.2 MB (22214800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fce215ecb937435e92000bf5dfe52f3717f5dca30b710c5064233ef875426f43
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73391816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d378acba0577367ce6a31afd366988b2b397f9537de3a47b965ec3899cb758`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:56 GMT
ADD file:c18e09bd64c99d045a504c333efaa05322c76b488039b206edcf75aa2a1a3812 in / 
# Wed, 11 Oct 2023 18:25:57 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:49:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d2c869ca968be69328dfec29874eb48a467a69cd422adc8efeb8becda0764bd`  
		Last Modified: Wed, 11 Oct 2023 18:31:12 GMT  
		Size: 49.5 MB (49505948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237c6272beac4c07d1304257bf58d3b820f2122bcbcab4b1b528ef058cb4c81`  
		Last Modified: Wed, 11 Oct 2023 19:56:46 GMT  
		Size: 23.9 MB (23885868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6c5a3c841432a3311b27c5d3b9ab74fbfd33f1fc8c9c5570adcbd1a3449f301c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75645770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b139468ba853f4e64f72ad3a626476ad17acf6b17286e5b697e458ab16986cd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:e8e1c13db04ddce5a6b3f4e29283e75eeecf85f213c2433ccb342a253457abc1 in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:16:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b15be2fd60b9adae282f32076fd2c71211d17ebbacfcd05f447fd925da0b81a7`  
		Last Modified: Wed, 11 Oct 2023 17:49:04 GMT  
		Size: 50.5 MB (50485267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723c0728b8af72632afafd3935c3ba7ea6efc560054e0c90b0e9ac50ffb83d95`  
		Last Modified: Wed, 11 Oct 2023 18:26:25 GMT  
		Size: 25.2 MB (25160503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:630fa9a87431d5ef63ba0403e35b1d13078e44716350c2f7f626b79644299959
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73189227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f8b088028ae199b72c712652c50ff8948c76437c673b92447dcdf542c35ff8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:38 GMT
ADD file:b80f07fa17341655abce58a1824ae94b2623d66b3f37a58194b8a738cf645945 in / 
# Wed, 11 Oct 2023 17:52:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:36:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f19fff78c927722277ff3254b811f343062ed8e219c72e6938e3662c09994cc3`  
		Last Modified: Wed, 11 Oct 2023 18:04:05 GMT  
		Size: 49.3 MB (49300361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15bac615908c95055b5313c63aafda011d597eca6630f640261a9fcb21dbf24`  
		Last Modified: Thu, 12 Oct 2023 00:01:50 GMT  
		Size: 23.9 MB (23888866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cd232f49802d24b109a6845c69de40da722b1c48414c6b7198c904425c111923
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79394432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff07d1542982f90245cadfde4cf3d10fe51356a3b06794d5b5de4fb83cb01e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:45:44 GMT
ADD file:5f062baf648f8cba61d84347ebedbe11eca129a318a8146b4c7c30586cbf0436 in / 
# Wed, 11 Oct 2023 17:45:47 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:25:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba8528ad854acf64973cba0749a6cf58ce475318878f99dccc45c01a8b19dafc`  
		Last Modified: Wed, 11 Oct 2023 17:52:11 GMT  
		Size: 53.4 MB (53418284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271e36b4d4e036584f3b2cdbde2fbfbc08b9134b8b07ed792b7e85266c0094e2`  
		Last Modified: Wed, 11 Oct 2023 18:39:33 GMT  
		Size: 26.0 MB (25976148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:463277650cb87ff963c4f3e246c78101c2bf595bfdcfda04fb4db350e9dc1592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69007846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d4dea6048745e0f58711f73e97cfebd76971edb90fbbf0cf7dc14a24ec144`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:43c6868e1269e7652a2de8a9524ef2cfdc486ebee9b841c762abc68d593b7c7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73502003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbc0b99dfdb875d8a7fc97b0162f802cadba9a8045b9077107c5592300b2f65`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:51:43 GMT
ADD file:66653f97d007e397b8dbcdca1bbb32bd8039456ae5b2cae3e049382489afb265 in / 
# Wed, 11 Oct 2023 17:51:47 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c682795de2323b695b3a151f23480c972ce25be65bcc04708dd6eb7250c65b8`  
		Last Modified: Wed, 11 Oct 2023 17:59:19 GMT  
		Size: 48.9 MB (48923705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5035b89544b06f157cc1fcccda207a6403d5570c3f7b39d2148ffeb92933b0`  
		Last Modified: Thu, 12 Oct 2023 00:36:45 GMT  
		Size: 24.6 MB (24578298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
