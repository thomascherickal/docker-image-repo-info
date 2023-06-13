## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:1d1e3af391648896284d2d89b9a042f609b1536331520f78ab94442a8a82a3f8
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
$ docker pull buildpack-deps@sha256:dfe7021035dffe0c138118754b037ba069c93eaeb755fcb02bd76d898b85bdb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138106624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87827f704ac4b58c7958aab17d56cf2fa9f725a38d4ca72c1d665015fa6fd2a8`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:22:34 GMT
ADD file:8ed2c72091b90575b320038c2ad715760d6382aeea5c416dd16f7ed04e955217 in / 
# Mon, 12 Jun 2023 23:22:35 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:34:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e79cba44192968ca6ea42058e67723ae58bebd2ea54b31f432b1ffed9fea9d9`  
		Last Modified: Mon, 12 Jun 2023 23:28:29 GMT  
		Size: 49.6 MB (49551965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda7b25305de24c8cc4e88d990c3c3c70e109b190f7411b9d3237528081a161`  
		Last Modified: Tue, 13 Jun 2023 03:39:26 GMT  
		Size: 24.0 MB (24019326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c71d2bfd3c86199eb06493b2f6d0258d7576aca3f851198b940bb3b1505989`  
		Last Modified: Tue, 13 Jun 2023 03:39:43 GMT  
		Size: 64.5 MB (64535333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:23e6dc0298ac481fad9cb7116f79dedfc805068d28a70e11e38511c2c7ca63e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133189624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:527bd14ea7d79da0392582dce31d28e1745e84b6ae81cd6876bda4b4c63b76be`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:49:10 GMT
ADD file:b79d69fc6594f6ca5e9e76165017858724482b88aa3aa49e3db7b07a3dcabc0a in / 
# Mon, 12 Jun 2023 23:49:11 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:40:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:40:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13ee4e7971510c95d7e625030699b854921da16f6d5ef29884b269a308a37afc`  
		Last Modified: Mon, 12 Jun 2023 23:52:56 GMT  
		Size: 47.4 MB (47417325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8374a5ed08b072c6f518c88ddf07dd3d9e04e3ccc51d0810b12cd2ae53c998`  
		Last Modified: Tue, 13 Jun 2023 07:44:30 GMT  
		Size: 23.6 MB (23622159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640f3b5ffb5f4fc9722d6fca3f771a8db79e177cf1b0cfd035587f4d4dcf4ae`  
		Last Modified: Tue, 13 Jun 2023 07:44:48 GMT  
		Size: 62.2 MB (62150140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:805d2e28a1a9f76587ad3ed5540f29d4b12099828945a35ce3e7f904294b5874
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (126957177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3fe347e5a4a7843d35871d6eaf9152bb58c9f0b2caa65421054ffbea53efbe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:00:33 GMT
ADD file:82567bde3caa9ad83c0c12c0525e6fd51cc833f0b29e733c2da572ed00150220 in / 
# Tue, 13 Jun 2023 00:00:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:00:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:00:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1d80e7ebc54969ad575378cf66dc58999cbf341e0d2a92c9ff0bfd5b3b9fb1c3`  
		Last Modified: Tue, 13 Jun 2023 00:06:30 GMT  
		Size: 45.2 MB (45234838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a26e461ec0e64583c2acfbef48942f57c9de9da65ff1a078a62e910baf3ce05`  
		Last Modified: Tue, 13 Jun 2023 05:05:32 GMT  
		Size: 21.9 MB (21922951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da543e1cb7517b023e6ef07f0f0385da6f0c3f832cfd7ade1c7381c2ffe580b`  
		Last Modified: Tue, 13 Jun 2023 05:05:49 GMT  
		Size: 59.8 MB (59799388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:32b08022da24fab3b21a8d7efb1a9a1068dae199e38bddff9c7960dc54483e24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137641250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27dad57bc107657d179bc35ca0a7f24e3fe129b37b41bc87f60b2dbf789c0798`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:38 GMT
ADD file:94f1432513f9a03b38028af02b1d1720fb0558559faf3e7f9d7097cf6b962056 in / 
# Mon, 12 Jun 2023 23:41:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:05:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8ba9ab3e6f12b9702649c2e0c7d78e22ffb9183f68c288b9edef2387bd8d4efd`  
		Last Modified: Mon, 12 Jun 2023 23:46:36 GMT  
		Size: 49.6 MB (49592096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393fb89bae1d5f0307a283cb7c3b5f54cc63fde2e90b7b65ceae29bcd27126f5`  
		Last Modified: Tue, 13 Jun 2023 03:10:09 GMT  
		Size: 23.6 MB (23558237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4483fcef438011d245d9be3906ab5e6a92c139027fe4286dc7e46b975299183`  
		Last Modified: Tue, 13 Jun 2023 03:10:24 GMT  
		Size: 64.5 MB (64490917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:27c1736fb433a5e831c56799d362f7d766b146b3da305ed4d146e06c145903f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141776767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:889767edeae06a9bab5825b77d2774b4b4add1bd696d3cfe8be9c5df87d74041`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:10 GMT
ADD file:209e3bb955801ad81eb18a280f9fbd5500a0e1f04565e6c94c9cd24dcba4c0af in / 
# Mon, 12 Jun 2023 23:42:10 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:09:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bce10b6f772acc79b03d87add4bd359f98c767e3599f82d8e351cced14c1a11`  
		Last Modified: Mon, 12 Jun 2023 23:49:26 GMT  
		Size: 50.6 MB (50562699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d6b7d433b6a8b07b01e4b262b82f2b882380e41bcd3a6e8b88ca32ea66321e`  
		Last Modified: Tue, 13 Jun 2023 01:15:14 GMT  
		Size: 24.9 MB (24858532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1c9493cccdfcd2c44a013f62ecc08283137f3fd2d7a483cf56387dc987b536`  
		Last Modified: Tue, 13 Jun 2023 01:15:36 GMT  
		Size: 66.4 MB (66355536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6a30400fa105430ddfae617816508db73d346096f5709ec5aa7d02b9b34ea741
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136617452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bc12f0ebe210aa0e7d2eb9f2960437b6216f3ad07c56c3f5af8ab65d1bc7ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:12:52 GMT
ADD file:b2a9cefcdd223b4cbf9b1abac81e8c0c158a24f9c272910a8822619ea9d55ae9 in / 
# Tue, 13 Jun 2023 00:12:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:13:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65733d4f161a7d2fd9cef6d80eb7fe00897e936eb78d018361809f7384b08c28`  
		Last Modified: Tue, 13 Jun 2023 00:25:52 GMT  
		Size: 49.6 MB (49561285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cac982d96cd0724a1a282faecd42ae997cf2e6c468441bdcf2ce718f092f4d`  
		Last Modified: Tue, 13 Jun 2023 02:26:09 GMT  
		Size: 23.6 MB (23606470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec621985ebc463298904a643b89d8805cdefe9a156edc65db797295bf5ce37d`  
		Last Modified: Tue, 13 Jun 2023 02:26:58 GMT  
		Size: 63.4 MB (63449697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bea654d92632e95c17ef30339a771535fb1ba666c966dcc7f9e7e997f44781e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.2 MB (149217309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a196d599c231d808d1d63b16588e70a2c2f4a4cbaec04236d844f3df17207b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:19:31 GMT
ADD file:aded196ce7e0c005fe55d5a92492be8cc5d7934fac082b7ab95b8c946e71e0a2 in / 
# Mon, 12 Jun 2023 23:19:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:34:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:35:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3f8e732e00762188b5ba00db7db3f36c97d0fccdf3d6121db4ca1febc7d190`  
		Last Modified: Mon, 12 Jun 2023 23:26:13 GMT  
		Size: 53.6 MB (53558517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3615faaadea50ed31520dc05aeaebf1283ee0aae09227fb97c1a9de87beec2f8`  
		Last Modified: Tue, 13 Jun 2023 07:43:30 GMT  
		Size: 25.7 MB (25673673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdc90af7293b0d3b333a9a6a8a60e61400bc5577336008e14e772e6041c6bce`  
		Last Modified: Tue, 13 Jun 2023 07:43:56 GMT  
		Size: 70.0 MB (69985119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:97d23ce5ca156ad9c8a9674a344c308c3c2327b68200a337edcb85a37a47bb40
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127963856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f598b738b3fcdf18c60a5209d925b472b9366201b4b7bae3da85749d7c151b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:05 GMT
ADD file:a70ed7f2a74611e58dff0d33cfe5096adda0510365aa0e8d263a6b37246bc262 in / 
# Tue, 13 Jun 2023 00:09:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 00:34:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70731a0001323eb925eb073dd2d04510ef4700ac6f50030dfda993464aeac07a`  
		Last Modified: Tue, 13 Jun 2023 00:12:27 GMT  
		Size: 45.7 MB (45744069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd3aa3980443f31b6ef037bb0103dc68fed3f80d9dad50456dfc523c6e96bd`  
		Last Modified: Tue, 13 Jun 2023 00:43:27 GMT  
		Size: 22.2 MB (22237741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c649750d7b93709631b4e4968c598a571877e20cf0c740450004c294ba0fac93`  
		Last Modified: Tue, 13 Jun 2023 00:44:49 GMT  
		Size: 60.0 MB (59982046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3cf1bcb7e10c78b5b31371ddb8d0f3b8ac53d6f9d8ab9ad2dbce5630cd5d2b00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135558724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb011ebf9ef93c20a7e044defa3dc64c0b660e36de3ea642c41864b358c748d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:54 GMT
ADD file:7ea0e5c460c626891cd3fc90639d6bfb9a27beeb7f5c79fd9c348c5b6244bd0d in / 
# Tue, 13 Jun 2023 04:30:58 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a129144c9fdcf79f6394b7f7bfa3d7e6a0c8ebfd424dca918695356a1b3bf970`  
		Last Modified: Tue, 13 Jun 2023 04:35:27 GMT  
		Size: 47.9 MB (47920583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d42182bfe271810fa332f879c12433ca046660729997bdce646aa7157138984`  
		Last Modified: Tue, 13 Jun 2023 18:39:25 GMT  
		Size: 24.0 MB (24020404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b53f300fd0adc6e321c844bd2e2fb478de90848743069202361df4928dd446b`  
		Last Modified: Tue, 13 Jun 2023 18:39:39 GMT  
		Size: 63.6 MB (63617737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
