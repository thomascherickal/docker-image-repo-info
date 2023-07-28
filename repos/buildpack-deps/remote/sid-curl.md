## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:8911799b59af6f47e801d0c01cf2534bfa5539eac4050cf8a1a458fb569dc6ca
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7d2668493b4f046b71c6260d3279c31c6ba4f2a286b05c50c2f5b4e868e1cf3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73749616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6413f0d2d0378de2d6a8d9d1402a6084483971c14f3fd113e9eb890502af0b02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:391166be1b5051ddf6888b026954e2ceb91731c8f106c47f53467f9d6c01c0a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70179798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea062241315ea22f51b37db746abfaeff210839177f580cbf50286096f670a90`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:49:08 GMT
ADD file:2673f00e844880d10f415db6b62b0d8686b31b02fca062ce8f3f69f12a911daf in / 
# Thu, 27 Jul 2023 23:49:08 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:23:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfd23d2efc358b5d10dee265443e93a7ee2f8ba25de718f6768468d3633354ae`  
		Last Modified: Thu, 27 Jul 2023 23:53:05 GMT  
		Size: 47.2 MB (47221377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b4f87496ef8bdf1448a907c4d6536736135506ae895a3f8c43e54abfcf401`  
		Last Modified: Fri, 28 Jul 2023 06:27:27 GMT  
		Size: 23.0 MB (22958421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:38cefc4528dfa54d7d2c303a875d83783caba2885f0e0c50e7a007dd9359edfb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67186352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d3e7ef599293db15f9dc303f0ca84c0f3f780d34d48a1550b46218894a7e72`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:59:54 GMT
ADD file:751198e94159fde0051292c0a2bcc0ae0c4b82b34b63913cd6860cbed520b9b6 in / 
# Thu, 27 Jul 2023 23:59:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:04:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8947caaed239612a0bd233bb275a710201bd19a169719c1541890b12489b8ff`  
		Last Modified: Fri, 28 Jul 2023 00:06:07 GMT  
		Size: 45.0 MB (45003207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96bf8c5e8d5b1c11dc8c30975084aa14717c1f1f934dac2277e9e70b442786`  
		Last Modified: Fri, 28 Jul 2023 02:09:27 GMT  
		Size: 22.2 MB (22183145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3365070e82e069764da8c54e5d427b3a3d1885114851410b82fac733e3806447
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73207925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32906cbdfc3a1ac90bb1eb27f714cbc6541ad954cc5d7d88a8515bd8f459f6cd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:44:04 GMT
ADD file:dcd44d784a7d0453b2aba140a48cea6ad00cd9860ae3735af4f338a7e242bcc5 in / 
# Thu, 27 Jul 2023 23:44:04 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08e4368591339a72e0b1d1f2280b8e4ec99150999d73beaf90f0bb0f074ac3bc`  
		Last Modified: Thu, 27 Jul 2023 23:49:07 GMT  
		Size: 49.4 MB (49385801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5715207583ba2736d4e317a197d452354d90b2b0974635872ad69588c6c1c6`  
		Last Modified: Fri, 28 Jul 2023 01:44:37 GMT  
		Size: 23.8 MB (23822124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:555e0c926152f63f4be81642923a7d416a6db8de6cdeffaf232ce9a51950f704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75427637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43878012a9d69af31988db85d06eed454cfed8f9f71f7baeaf892725ce675e3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:40:19 GMT
ADD file:565f8487c71b5de967f1bf16d4bd86291107b68f4152a61e35a8ab86e9f83b7b in / 
# Tue, 04 Jul 2023 01:40:20 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46685592106ba6554716942e180f6b4cd8a73f1ec934554b40aee89b47118f5e`  
		Last Modified: Tue, 04 Jul 2023 01:46:32 GMT  
		Size: 50.5 MB (50505825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf3084ac7ee091f26af470878c8197f67d44c09670c27921a26209c909a5c0b`  
		Last Modified: Tue, 04 Jul 2023 05:42:02 GMT  
		Size: 24.9 MB (24921812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6d22f564936ef6047f439f288c6487d49ea9ea94a3d3d823ba789aae0b57477f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73200135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73a82efa8a0cbd2145763c100f743ab0c6073cedbe7ab03288024f57dd678d67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1011282f636699406a5310ef60be3fdc27eceecaca0896c8a5bef27734e089ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79319025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d91219a38ec64926ab216585e4d2a7d79f6502555b74c1e31d29c6605712dd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:36 GMT
ADD file:c9a8e26186be211989debc20aaaea2b9b0a88ef3c95dc67df08fb292c70fd107 in / 
# Thu, 27 Jul 2023 23:24:39 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:56:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a2370b39a2d35f89bb2978a591923ded0652ff040aa00a837d799ffdb028e76`  
		Last Modified: Thu, 27 Jul 2023 23:31:58 GMT  
		Size: 53.4 MB (53379244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d10ad7881963b1a20b168e2bcb81ece809f0540619df3bc4c580ed5340359a`  
		Last Modified: Fri, 28 Jul 2023 02:02:37 GMT  
		Size: 25.9 MB (25939781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

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

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6ad71da42ad5ba3b2eabfb86b6e5f739dcbfc42fef75faa3731f74478049f508
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72158449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d38ab10dc02fb9498f17ee9b5fe76fd640f18194d11b931c7d906c6499d0919d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:26 GMT
ADD file:b143b1c75d100b35ca10aac97e0e6b44c6dc267e1c00c3fa2f3f3dd3c408809b in / 
# Thu, 27 Jul 2023 23:48:29 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:59:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff8109f0f7ac0173229961049cf524677815675d18f6769369db2d95049f4655`  
		Last Modified: Thu, 27 Jul 2023 23:53:27 GMT  
		Size: 47.9 MB (47858669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f879bcfe385fa3b5dee9245ad57b8b234bad70af78eef788bb04fa0802b62`  
		Last Modified: Fri, 28 Jul 2023 02:04:03 GMT  
		Size: 24.3 MB (24299780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
