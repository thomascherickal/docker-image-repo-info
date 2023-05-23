## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:b65f8eb435a27a1db4f440073e576d6b429309d1a693b37078c65f0b47853331
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
$ docker pull buildpack-deps@sha256:51092cbec226f662a97ab8f224f1c6a22c784015b39ebbc06812a0828a22b0ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137682711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86552ccbf7feeef5f1324e901fcc4b77049d31af9ced94638b9fbd1fe3fa7fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:19:36 GMT
ADD file:aea4560c39a3a877086fc63afdf218ba3600a05abef7c44563f788e8b60c04ef in / 
# Tue, 23 May 2023 01:19:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:45:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c98dda1b0e97e7fa61fa33cea43f85bb1a36a4f6f65c7b8430cae442b76ece09`  
		Last Modified: Tue, 23 May 2023 01:23:14 GMT  
		Size: 49.3 MB (49301275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a463ac54ed3eeee295443fb87b28643b95d7975e83bd214bc93db462b1b59de`  
		Last Modified: Tue, 23 May 2023 01:55:08 GMT  
		Size: 24.3 MB (24274092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7076663891554c4b6516ec84fd2d5459502966e94b4d794796b086aea4f4ca2`  
		Last Modified: Tue, 23 May 2023 01:55:24 GMT  
		Size: 64.1 MB (64107344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e47b720b35ad887b644c94481713f1d2aeab7646224b6b5084d767cea5479613
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131671128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe93bb920dac94f750d11119c6fb44d3e36fe4979b953b01468151f735a7bb4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:48:16 GMT
ADD file:8fc8e3b90ac0435374d713c6b80b23f1db0866a447cf839ea8304d4717982da3 in / 
# Tue, 23 May 2023 00:48:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:12:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd47f968dbd1b839925549bb9a90d021c19486875443123fb77e8cb1367e9745`  
		Last Modified: Tue, 23 May 2023 00:50:22 GMT  
		Size: 47.2 MB (47168971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dcd7a31d73fae7c8f3da6415b83f56c0b8c1635526741fd0c65632ae15973b`  
		Last Modified: Tue, 23 May 2023 01:20:37 GMT  
		Size: 23.0 MB (22950966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64527cb5109ec935f8bef268d9948c57924a7b5d1bbcda29e980f1bf4a6a37f2`  
		Last Modified: Tue, 23 May 2023 01:20:56 GMT  
		Size: 61.6 MB (61551191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:84b42b9ed8300cea840175d87c8ff51940928c0e26337fab6c27910588206350
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127463114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bcc6f9e63b42972b8b5f9b4f62623a5be08255432e153a6755aa3c57bcc46a7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:28 GMT
ADD file:222aad59c348a6e07dd607ba4626497e12e5054fb651c9c30d5a4c5a8b3e4c82 in / 
# Tue, 02 May 2023 23:47:28 GMT
CMD ["bash"]
# Tue, 16 May 2023 23:59:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 May 2023 00:00:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:326cff266909348fa4e168fc7e76fbd52cc4855403565526a5ecd2e6bdb9d26c`  
		Last Modified: Tue, 02 May 2023 23:50:34 GMT  
		Size: 45.0 MB (44988072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abb83f097438eeb001ad7afc4116735e243a512d7cfda49cdb7b6bd1f009b9`  
		Last Modified: Wed, 17 May 2023 00:23:16 GMT  
		Size: 23.2 MB (23218068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f50f8d763268ba1b4d8d7363b0b478fbfca7dcc73fca7947c65853b1788813d`  
		Last Modified: Wed, 17 May 2023 00:23:39 GMT  
		Size: 59.3 MB (59256974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1e4fd4adc8d135512fa0806338069ddb4b2e8d4a239752529bfdeb2edec2fefb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138229402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b810d068f2c2ddbb0ac47a859b6fc4fe6dab6f24c229855085bdefded0a84202`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:25 GMT
ADD file:1af23b8894efa507a47bf873cf69ecaa5ea13b618cae85b8c46125af6399b4fb in / 
# Wed, 03 May 2023 00:22:26 GMT
CMD ["bash"]
# Tue, 16 May 2023 23:39:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 23:40:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15c964cdaf05fdeddcf9bddd79eba05f71f2859fee9c193ba5d19a237f7fb92e`  
		Last Modified: Wed, 03 May 2023 00:25:01 GMT  
		Size: 49.3 MB (49345335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1426a52e9479646762d18e7a8f0b801f6ba0cd16196e4619fd66dee64a27715`  
		Last Modified: Tue, 16 May 2023 23:56:18 GMT  
		Size: 24.9 MB (24898492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd095d9f8a0dbe9574d92083852c11e0a6a6cd230364b19fec3cf45f8388a33`  
		Last Modified: Tue, 16 May 2023 23:56:33 GMT  
		Size: 64.0 MB (63985575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7285ecb58abaacd425e46a8f49f8848527e92124aca75931d3946c1485e6553f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141403547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829e40641db120e27b6767c9d5834e7a3fa2066af32effc700c78a83725e9393`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:38:43 GMT
ADD file:4d14207b5cf935fa2b9de70132f41a0eb90a8b5200ed3d27e60b766fc6131e13 in / 
# Tue, 23 May 2023 00:38:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:54:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22e40771358829b6817b47cb2d682b51257385478c18bb1ec96251a68a9c75e4`  
		Last Modified: Tue, 23 May 2023 00:43:23 GMT  
		Size: 50.3 MB (50323189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bf109a603c637e9a80a5a8fe46353089a5fb8c6333eced350af89d7298576`  
		Last Modified: Tue, 23 May 2023 02:03:46 GMT  
		Size: 25.1 MB (25110482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39204aa4c310e5b428093f5182d87e2f302dabb686c85507aed2372505156242`  
		Last Modified: Tue, 23 May 2023 02:04:08 GMT  
		Size: 66.0 MB (65969876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a28e3e52d5e8501460ad0f433ddd327754cef7c299876082bf8ceee5d0ecda35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136117227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5261b221a9ad12c69fa02f279869a63b04bdd93b9fbf19edfcddac08408b9de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:07:59 GMT
ADD file:c8965d5e1a440e4bc93318be2f80c95e9692ada237122031d2e98793b8036143 in / 
# Tue, 23 May 2023 01:08:06 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65775e721f6c7f76e54f65c03408a249103c86c536e6a86498f9f5a6229b9f4e`  
		Last Modified: Tue, 23 May 2023 01:17:24 GMT  
		Size: 49.3 MB (49304239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464924f070f4f4c8a4e8facea0026336e200a0c517951d62854dc3b3a1154f58`  
		Last Modified: Tue, 23 May 2023 02:06:54 GMT  
		Size: 23.9 MB (23864351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359f2eaa37862504aa49ac76cb23ed1f915f986e4579bc54affd5a7e8ab8f277`  
		Last Modified: Tue, 23 May 2023 02:07:44 GMT  
		Size: 62.9 MB (62948637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a70fee0093fc78a9ced3f519cb0f01aee68baedc6ac1f6a1afa1cc11103d3ff1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148803187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e212d4fafe68f0c10626374ccb6d62ba1b8d22f76d5b5913300ed6cfe2ba0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:16:38 GMT
ADD file:28e774b3554d274fc742feac48f78a3bf6f120cb729e2824007dd94d5c414156 in / 
# Tue, 23 May 2023 01:16:40 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:45:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:46:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e109feef3fc6307cd9a880958cef6624de9c2c6f054987e479461a1ae51c7503`  
		Last Modified: Tue, 23 May 2023 01:20:49 GMT  
		Size: 53.3 MB (53312324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab84a55cc084469df8b38ab6a01658bfba2b29b7410a970ba6d9d2864846672`  
		Last Modified: Tue, 23 May 2023 01:59:19 GMT  
		Size: 25.9 MB (25923867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfbe0bc6dc85168e7da83a7be20c9913921338417e0c639a93ff1cdc5664403`  
		Last Modified: Tue, 23 May 2023 01:59:46 GMT  
		Size: 69.6 MB (69566996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7a1f44bc69e4fdfdc35cd1132e60cf090df46229f85de4e53b154c450409294f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136141105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d776cc668adc1cc56929240cc2477c0d11f991b60f4113c992f0164ed452121d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 03:41:05 GMT
ADD file:2b13279140b98de657b363865f9ee14f0c5c26df191533d1c5438dd1df5948ca in / 
# Wed, 03 May 2023 03:41:11 GMT
CMD ["bash"]
# Tue, 16 May 2023 23:41:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 16 May 2023 23:42:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f966d911ea531e8d55499ff0d85338412ff6e8012a1639d691e4bc5ecf08d42`  
		Last Modified: Wed, 03 May 2023 03:44:23 GMT  
		Size: 47.7 MB (47675931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a0c25941897af74b548e8b3030a4f6d12d7e0540497c20305c519e8b6a89e1`  
		Last Modified: Tue, 16 May 2023 23:54:59 GMT  
		Size: 25.4 MB (25354263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c26bb6b06f66508d8f39d4e0ebc7216ae69662d6a748faeb8e1bc37e112d24`  
		Last Modified: Tue, 16 May 2023 23:55:13 GMT  
		Size: 63.1 MB (63110911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
