## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:9dfd5ce94f1691a8f76e3327998f4ed29af94c0f18714444983544005ea69e18
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
$ docker pull buildpack-deps@sha256:8a363c27455cd9f6fcde5596efa71102fa5c2cebfbf12fb0c5157e2fd3ab60b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138424099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4cd89db58a3ce0a728b12a56803552a04aa7aacfc0b27734d53addf8a3d8ac2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:e32deacfa38b7c02986a841b125a79769d3d74c100e44c5f5b142b35e13831a4`  
		Last Modified: Fri, 28 Jul 2023 03:10:34 GMT  
		Size: 64.7 MB (64674483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:58bff3fc0599443e68fbde0709beacf8f49088d7a7a09e747494c2ce064589ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132473799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383cad8813cb0d3a326b121204766800dbe924af98a27516ce6a11478476b5af`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:49:08 GMT
ADD file:2673f00e844880d10f415db6b62b0d8686b31b02fca062ce8f3f69f12a911daf in / 
# Thu, 27 Jul 2023 23:49:08 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:23:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:24:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:00122d9d2372df69cf047d7f54472fb364cda9c02748c185f9da615a327633ba`  
		Last Modified: Fri, 28 Jul 2023 06:27:47 GMT  
		Size: 62.3 MB (62294001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0f95d00314dc39f5dd6cb7b204eda7bb9c5ea26d460c27c8c4da6d14663c0f22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127122546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b6dca471b15c80f727a4e9acba1011dd916399bd5d8cdd6f6ba849f57d684f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:59:54 GMT
ADD file:751198e94159fde0051292c0a2bcc0ae0c4b82b34b63913cd6860cbed520b9b6 in / 
# Thu, 27 Jul 2023 23:59:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:04:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:76e7aeb6f855e0c83f2b3af5949abe078751618c4af65d6476e5d01a662d8f4e`  
		Last Modified: Fri, 28 Jul 2023 02:09:44 GMT  
		Size: 59.9 MB (59936194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7332010e16c7a9cc11baf0299b5bd955e48cb1dd5830562c20c2e0ea10321578
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137836200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c78d6db2ace16a5439289ed8e6f9ddb461e2c565d1be0f96f85c19ba33fd779`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:44:04 GMT
ADD file:dcd44d784a7d0453b2aba140a48cea6ad00cd9860ae3735af4f338a7e242bcc5 in / 
# Thu, 27 Jul 2023 23:44:04 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:bcb506cc81f7b1d26a7bbb59bd8c08177f30223b1b321d36119bd3672ef3bc1e`  
		Last Modified: Fri, 28 Jul 2023 01:44:53 GMT  
		Size: 64.6 MB (64628275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:08ac98188b4d99022ddf9f16dc0a488ec35f19e9d09d3930aef1e2f733ae81d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141945829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6989e556ea04ee7a099cc0e1e2fa0719d9fbf6a8ce54cc152f9844ccdc9f46e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:40:19 GMT
ADD file:565f8487c71b5de967f1bf16d4bd86291107b68f4152a61e35a8ab86e9f83b7b in / 
# Tue, 04 Jul 2023 01:40:20 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:37:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ef6611c0dbf9970353c5c08585b89e28e50531495ee733b7f098fa9c3501067d`  
		Last Modified: Tue, 04 Jul 2023 05:42:24 GMT  
		Size: 66.5 MB (66518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:13c2f443dbe0048ee66a2dc9ba3c4726b576afd4987d853bbe4be5fd6c3035e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136780149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b5b566617eecf28afb7200ea107a9a85c4a5a8df702a8b6ef7b47930e217b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:29:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:86218b2ed81ed0041845b0b5b1e95efe348740465925fef57859a751cd7a6596`  
		Last Modified: Fri, 28 Jul 2023 01:38:35 GMT  
		Size: 63.6 MB (63580014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d395e639b08a58c92eaa4e579dd1aa5e2bf3ac4d1a2d1066929e01c03476e2a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.5 MB (149453925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f60e01be4d2e40e746fd9f10799451c914761f965fcdaefba640b3ccfb2eb9de`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:36 GMT
ADD file:c9a8e26186be211989debc20aaaea2b9b0a88ef3c95dc67df08fb292c70fd107 in / 
# Thu, 27 Jul 2023 23:24:39 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:56:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:56:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a5a7ffe37ee9b72d23063d94fa331f2cc24e8756c3848a55df61f93481f3fbe7`  
		Last Modified: Fri, 28 Jul 2023 02:03:06 GMT  
		Size: 70.1 MB (70134900 bytes)  
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
$ docker pull buildpack-deps@sha256:12c2b36704dc97a00fb11e6f368e03ab55455b19288e6a101d4c16ee6ce63732
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (136038066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b1e80b6031d963198ff982d8a610e3990527f3041004a2464f3e0743c8fdcb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:26 GMT
ADD file:b143b1c75d100b35ca10aac97e0e6b44c6dc267e1c00c3fa2f3f3dd3c408809b in / 
# Thu, 27 Jul 2023 23:48:29 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:59:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:59:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:5daa176328aab710c51edf5d61e90473578a5a55c56a699cb47bdcae40f56313`  
		Last Modified: Fri, 28 Jul 2023 02:04:18 GMT  
		Size: 63.9 MB (63879617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
