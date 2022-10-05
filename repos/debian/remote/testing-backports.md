## `debian:testing-backports`

```console
$ docker pull debian@sha256:f228dd555085d505870f90806b13168466f68edc93e8721370489808464956f1
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:388b9c8b68ada0c0d004cddb8390053bf990b57da5afc03cfd7185cd238f1499
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52962717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd51a34cac415d97be779a686c60d6920428566cc31190366307b2358cc2c2a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:28:15 GMT
ADD file:0b13c22e675513ff50745105728cf4c7dd4f059e92da40d8ddc3c62846b90df4 in / 
# Tue, 04 Oct 2022 23:28:15 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:28:19 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:790bf367fb985fa8358aa0d545464d01c793d1a2b6ea53fe39e657deabaf429d`  
		Last Modified: Tue, 04 Oct 2022 23:33:40 GMT  
		Size: 53.0 MB (52962494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f76b7aa3c8c779d4476bca47a5886fe5a7c6bdb14e1ce45968990751551eb9`  
		Last Modified: Tue, 04 Oct 2022 23:33:49 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:ab5fe1ce53a8d8ce6f9228b3ffd8d859ee2ade75f7a949379da9c79e27c3395f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51838859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f6c2d8638fd6f730e7996d1b2a7398c937d0abdc6e48673af9af30478d9cc13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:50:08 GMT
ADD file:4f92208bf3c7e9cf487f789719e3f73bbd770730b682349024980b82a515209d in / 
# Tue, 04 Oct 2022 23:50:08 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:50:14 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e55f8a586de9d57d2efa2ee6334e444307fc037204eaad3d022a6b15cc681ae1`  
		Last Modified: Tue, 04 Oct 2022 23:55:38 GMT  
		Size: 51.8 MB (51838634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc6c573d00765072b12e0660f494d5a2dad260b15eef4a2b24af04684f90610`  
		Last Modified: Tue, 04 Oct 2022 23:55:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:5b450828b6ffcabb4d8241d40719ac88f2f87185f3c88be786b64e0227fa8bbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49692837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87eda27cbacd4257024b9ff1cad2fd859464c6ac2488fa53229b393d87e8bea5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:56 GMT
ADD file:ddc9f933740d9761a7df5d431009b4ea57ca7ccfdc696991396b8146487de6fd in / 
# Wed, 05 Oct 2022 00:00:56 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:01:01 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c3df8ed753a707fad4656d16393beb9198503102ddab60f8bd7c1ebe95d21d7e`  
		Last Modified: Wed, 05 Oct 2022 00:08:25 GMT  
		Size: 49.7 MB (49692615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a539de1fc6b6643ff8aa2455849f7c1575331cdb718998809fdb190ea921ae6e`  
		Last Modified: Wed, 05 Oct 2022 00:08:36 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:5353c8db079d868d6c96b2f932e94ec1f438924ca13cec37c51e649e295e3f42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52980621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bf2a79b62dfc1042874a53f23fd6aa0dc233299d1bf91c44cd4d29ab4024271`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:46:34 GMT
ADD file:d8a562b059284e25b26f8bb851509a38bf96a6ca745d5f220f0c50c5a2791d8b in / 
# Tue, 04 Oct 2022 23:46:35 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:46:41 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:76f19dcc19c7ebaa09b68b24e05232d803279cd70b2bfaf1b9b883b76e3a5147`  
		Last Modified: Tue, 04 Oct 2022 23:53:31 GMT  
		Size: 53.0 MB (52980396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd605a54635e20f4be7cf40fa4e1797422e1125243d99991e456e9f2d39e0773`  
		Last Modified: Tue, 04 Oct 2022 23:53:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:422c12a384ab84aa84460192cae0619dd1a1e23c735ddf81fe941ef524222eaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53933037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fc996c440fa04acdd0fc106bdd2f5cdfff8d35dfc4e2bc02c4956c2a7d06f14`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:41:37 GMT
ADD file:4db100bfbc465a525abe69bff13a338757df520a3ea1a2abe2aa32e24be3eeef in / 
# Tue, 04 Oct 2022 23:41:38 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:41:44 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2737ba33022030f9540c96cf5cd6196d1696499b8e686f0ca9570e214168446e`  
		Last Modified: Tue, 04 Oct 2022 23:48:43 GMT  
		Size: 53.9 MB (53932814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e0549c206029256049c343b2a681852cab520f4e9ca7bd416b3a0841b386b2`  
		Last Modified: Tue, 04 Oct 2022 23:48:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3ae2b45d3dff79ed6a64eb192df8ba79cc7550738630ca6941ccf89f7c1a9104
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52967232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32cb1055829163e06706f6b57c6d3b1d9101f2ac06d7ff9b7f65eba069f1b4c8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:18 GMT
ADD file:4ff9efc8f665301da37db96a22470e284e0d7d47891026e9194a2c7709508b8b in / 
# Wed, 05 Oct 2022 00:13:22 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:13:34 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1454aae498a3aa762b432635fb671c490406bf5e6ec9ca85aac661eab19b190c`  
		Last Modified: Wed, 05 Oct 2022 00:21:50 GMT  
		Size: 53.0 MB (52967007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78aa87929f162f1fa06c0dd2992068d599de529c3636920fa06651e4215a8bb`  
		Last Modified: Wed, 05 Oct 2022 00:22:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:1affc7ed9c882c07d227584e568dd56da1467edace36729b244967a9934f02fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57111756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5612f6f62f75f8be917fc1e1ab6891a1dcd2e673acedc97ae25b531922fda640`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:19:42 GMT
ADD file:21bc77855660325b0bbe95ae9c594f1a8b6f5e51d157ec61f68fb21e07bd789c in / 
# Tue, 04 Oct 2022 23:19:45 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:19:52 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8fe8d5806e08283bb0c9e0e9b0692bb71119a514d7b5abe7e35e38ba3dfd488d`  
		Last Modified: Tue, 04 Oct 2022 23:26:28 GMT  
		Size: 57.1 MB (57111530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099b14c72b43fc6ae8749c5b94a3aa4767a1d1ee807eab7c0f29a5bc40e8714`  
		Last Modified: Tue, 04 Oct 2022 23:26:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:9a8b2a74dca10f43ca775543962564284130cf4712b83a40ace92ebd6f7894aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51280365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933ab08e3d232128c0867a968f0b3fe1f3be40eed06ce2eada4407ae59e8281b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:43:51 GMT
ADD file:82fd108325a4206c09989fb611c03498babb6258eb453241d2d4206b0a1715f9 in / 
# Tue, 04 Oct 2022 23:43:54 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:44:01 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:749658c1e57bd3baf981210cc7dfa16cc15383c08d876c511d08dbd7f0f45844`  
		Last Modified: Tue, 04 Oct 2022 23:48:22 GMT  
		Size: 51.3 MB (51280144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85033c48d7b3040bbd6d5acfcf5e82d9b45e9f379cff9ff78f3e883927d55a1`  
		Last Modified: Tue, 04 Oct 2022 23:48:29 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
