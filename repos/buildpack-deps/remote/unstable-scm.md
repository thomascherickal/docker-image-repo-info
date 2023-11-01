## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:aaab6b697ef8824a2007d683bd566cd0be4028b10cd42af7238fa7d0f6d574fe
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

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:69b4c504c9caa677158b04a5dffa59425c7649f735a7b8728d6537f55e5bbf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.4 MB (139405504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea95fd684a079be0c5deeb96861c07b4992a71e7818a9c7960f6a1baee07c8f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:27 GMT
ADD file:69815228666696b3cd3b2799492e3d9cdf4f513ccca5c1cc9282f6c569cc8730 in / 
# Wed, 01 Nov 2023 00:22:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:57:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:44ee245293502f2c719e3e2302ae5289fe69631d1c3bc58055166bf026f0a28a`  
		Last Modified: Wed, 01 Nov 2023 01:05:21 GMT  
		Size: 65.5 MB (65516786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6e5665d5853aa13b18e4bc33e2e74ccd3fd4299bbee0d5638a8edfd8811fd31d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133155810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82733bdae381c5738d0e28f4d4a7b2e23a488cf237028a2f9d7340ed42a2de6a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:22 GMT
ADD file:32bc859b55e9b4aada411b379418b1cd95da1e1f72e89ade7698d0132f8edafd in / 
# Wed, 11 Oct 2023 17:38:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:c941934e31a404779530c5e75e27d66e4e8c42e849ac2f650b72bf46c0f1796d`  
		Last Modified: Wed, 11 Oct 2023 18:17:15 GMT  
		Size: 63.0 MB (62997933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0241422c180b52449cebfb843511a622b3db62b876adcb35f83687d33338ebd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127780532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e47cd5dfc4c910b811a8be1f25b280a059fbcfd20276ea41ecb9d61a43415c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:32 GMT
ADD file:e83473ecad5aa9a153d02c535c6e40e22679b973268fdd74a0f5bd86b004222a in / 
# Wed, 11 Oct 2023 17:43:33 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:50:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:51:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1125f5d06321662f68a43b031f5a38e65b2f62c0728741c6bf3b55cf2c66fde2`  
		Last Modified: Thu, 12 Oct 2023 03:59:44 GMT  
		Size: 60.6 MB (60612153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:944bdc970d6ca598d11e588a54f084da0fb8a9ba812e762a9214eabe87384929
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138977761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1834be5b56b00292a42bceb02448a4a30da604bc1654bd80098dd463aa4b5e12`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:56 GMT
ADD file:c18e09bd64c99d045a504c333efaa05322c76b488039b206edcf75aa2a1a3812 in / 
# Wed, 11 Oct 2023 18:25:57 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:49:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:49:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:371f902523aeade9aa8fc3b19ce94a0e511fc0c9643616c1d93df922a8fabc1c`  
		Last Modified: Wed, 11 Oct 2023 19:57:02 GMT  
		Size: 65.6 MB (65585945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:db6becb86617eec873cc1f2cbc1f8c0abd30edc8936fe15da22884a7c262b25f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.9 MB (142912216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5170e1fe625abd2d29e37453c2b4b9ba4255f5b27a6f1e529629d4b96d54a95`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:e8e1c13db04ddce5a6b3f4e29283e75eeecf85f213c2433ccb342a253457abc1 in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:16:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:17:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1b827bfd5c1ab262e6257af597a15e6fc633a0ea1ea51c3903247b98e8892a97`  
		Last Modified: Wed, 11 Oct 2023 18:26:49 GMT  
		Size: 67.3 MB (67266446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:89df672a2eae0669920f05fcd19c0581e1dece33f0bb2a1d319e25e9d2537059
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137502013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3b055ef2c6b884b963271c3f7fbb51f1913f3ac0ad28460eb6d5a0d022fb30`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:38 GMT
ADD file:b80f07fa17341655abce58a1824ae94b2623d66b3f37a58194b8a738cf645945 in / 
# Wed, 11 Oct 2023 17:52:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:36:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1cd7c4ef998d1377d5f93a0a39cb5883535c8632bd1aa9bde6b889d7aaa211fd`  
		Last Modified: Thu, 12 Oct 2023 00:02:42 GMT  
		Size: 64.3 MB (64312786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:353b2a9b54d029503ae0b036b97d823535850f152a54820f9faeb5adba83eb89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150372100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8e3c9ad7f10aec351582b84c48d9a4a2a4b8b4496b3fc285248982f5238995`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:32:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f87f5498621b44bb593666a49a2167487d185ef2ba48d24ee657724f9e1b8`  
		Last Modified: Wed, 01 Nov 2023 01:43:17 GMT  
		Size: 70.9 MB (70933174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:60c63e0e0ad978fcf73dd18012240127fcb631a7993d05b3f9d3ddabab132675
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139893138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f3debda305b48b4c96aeca9c4076cb44864a7a588e3041b287ddf0f78757147`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:51:43 GMT
ADD file:66653f97d007e397b8dbcdca1bbb32bd8039456ae5b2cae3e049382489afb265 in / 
# Wed, 11 Oct 2023 17:51:47 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:07:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:3d73bd759805634b041aa9d93b37a142261e1a8bf4ecb0b621c18e8e42879943`  
		Last Modified: Thu, 12 Oct 2023 00:37:14 GMT  
		Size: 66.4 MB (66391135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
