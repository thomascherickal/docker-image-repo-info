## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:90cdd994eda7ff669755374a85ad286f9a3f4e06edeba7a0e3ce40f52736f640
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:ec45ef53785038c4e6d78f094260df6b304f98b464733d64066f2df81f54a956
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55567481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8478ac217d3c676202cdf76fed12901ca8fe812d5f926315ed7e622ea9bc11eb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:47:43 GMT
ADD file:d564072c450ac56e020375a2295aaa9d2d8deb426d0a1a50f5a500fa401e7cb0 in / 
# Thu, 02 Dec 2021 02:47:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:47:48 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e4a54c5157321faded684f3a0a8bcaee56b08c45f1d38a4e0b0b690d7e1c98be`  
		Last Modified: Thu, 02 Dec 2021 02:52:41 GMT  
		Size: 55.6 MB (55567256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06aaa2a87a0443bca2089f80ddcbc3379f4e04f293da2786abf6d2fc236e075`  
		Last Modified: Thu, 02 Dec 2021 02:52:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:a50710df0380f67a284d2a2300f466f5056e344a617110f51a71dd6fb3fcca02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53031380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74706361bda1711805c7cfa34345529b2c12de4d83a491f8eb0704269b0ef7b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:00 GMT
ADD file:565dc0a92c6ce86500c032d7c7e8112f62771ff3bac3aa84192e8309ae7acbba in / 
# Thu, 02 Dec 2021 02:49:03 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:49:16 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:92dd04f71649984a91d8241840b2fa0a06cee72bebcd6503ece93ae1b5f47d07`  
		Last Modified: Thu, 02 Dec 2021 03:07:38 GMT  
		Size: 53.0 MB (53031153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901f9bdb26f2fcaf0ffa5c2d39c0ef10d210f8af310e92efa6b337b7356593a`  
		Last Modified: Thu, 02 Dec 2021 03:07:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a12111d3107afe6e5cba6bd7284ad5fac71667d6ebe9a86f756011c9253065ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50589242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fda4853768dab32f5ea58f84d28ab2f888e02017edd6c19a217ad3c23d1fe1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:58:07 GMT
ADD file:6def097172b517cba3f58db99b3dfb25785929bad969e154025a1db5fce45c12 in / 
# Wed, 17 Nov 2021 01:58:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 01:58:21 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6316dbdb4f8715ca0987361e8e193aa4f97570b0b307991e95a5bd5475b35ccb`  
		Last Modified: Wed, 17 Nov 2021 02:13:14 GMT  
		Size: 50.6 MB (50589015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a593cabba4a80ac3c0d10f1ebf5685b08a5ed4cd93a935e5663efe65cad1874`  
		Last Modified: Wed, 17 Nov 2021 02:13:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:553a3ea7b9ef880c02121ded7674510c5d8849df4f3cf72101e5b6612779b0e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54464614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7cc4f49d0f64481e618b845ce734645c1f9bb323be3496b196eddeda9d9a31f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:34 GMT
ADD file:cd982be7a5accd4c715a3de7a8682f869612c5401ec485ff4622a9590caf415e in / 
# Wed, 17 Nov 2021 02:39:34 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:39:40 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c646ef4eeacb8eade7583e3231bf320159c2c92b39835abd5631d8bcffea30b6`  
		Last Modified: Wed, 17 Nov 2021 02:45:59 GMT  
		Size: 54.5 MB (54464387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bcba5a68f6a2b8bcbf116fe8ea48697b964cd39cd77fe24a89c53d76f2d989`  
		Last Modified: Wed, 17 Nov 2021 02:46:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:d6c643359f4d99374111fae2c74932ec88fe216d1eb14915d2547b1f7000a5bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56610449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54a9576e8b945343b01e6fa1e35c58d4f146848c6c6d44b172b1c7b014095667`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:39:07 GMT
ADD file:233579a3cce5db7166a5e91e9473aa28283fe69ec6809ce49c166994ffe2d461 in / 
# Thu, 02 Dec 2021 02:39:08 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:39:14 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:66c36ad92a7d15b3332cd4cd2fd424021c2ce01463b45621fcab89004c4c763f`  
		Last Modified: Thu, 02 Dec 2021 02:46:31 GMT  
		Size: 56.6 MB (56610224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ee8179926ed6277b4acdb7617f830ed37052bc0b0804b77fe6f7f0947e0c03`  
		Last Modified: Thu, 02 Dec 2021 02:46:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:08a20159ed23ba78318d847b7fb8a5454caa8a351f8a6095c9833ae3e4191981
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54269820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb1d2a8812283847cb5aa15b80cb4ed890154847feef633408f59f14cdfc4eb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:07:51 GMT
ADD file:2b78b392bcc6daef3d9c93dcae4adf8b84cac89c57ed08bd43854d23774078d6 in / 
# Thu, 02 Dec 2021 03:07:52 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:07:58 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8c4a35c3e932252ccb2418c1bc14531f11d21f13ba131d0a52cd9cb690dc9623`  
		Last Modified: Thu, 02 Dec 2021 03:15:53 GMT  
		Size: 54.3 MB (54269592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a8ca1adf7665d8b56eb5f4dee37f9b21d2c8d750c93da7939bf44e64c9d2e`  
		Last Modified: Thu, 02 Dec 2021 03:16:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:9071efe09ce6d8e6a9b6b7226d8a205f5b266177c41c78598f833b14d090ffb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.7 MB (59706412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb59e9d3c59f71159bfcdac5dcb149b440289b4c1f08b42b845879d826978274`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:25:04 GMT
ADD file:fad90d698c5f566b126df2df0ac9c0abcdc50b5d25b2a1e33ae2e8aa18b9567b in / 
# Wed, 17 Nov 2021 03:25:19 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:26:09 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2de091795abecdff7dace8e57ee5679fae062a958230bcb89652ea0b3f44f240`  
		Last Modified: Wed, 17 Nov 2021 03:47:07 GMT  
		Size: 59.7 MB (59706184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c229d90083d4647f97c42e0f7feb12f8079d91fa6ff6dfbc0952f19e11cec9`  
		Last Modified: Wed, 17 Nov 2021 03:47:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:6b921b3ac95fa35d54bce79c71c521bb79945ce081dbb843ea590bcfaaa01352
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53669463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9a9322bbd38a47801edcbecc6975762fa99b8a17b3df5f0f0d24072a05ed03`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:36 GMT
ADD file:7913ed6a2385b3bfbd659a88c7bae1ef30f61c8147e8e89b5fc5c4be13a393ea in / 
# Wed, 17 Nov 2021 02:41:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:45 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4457396a5c3a0ebad221540b501d8baee17387a6ab52192d3b8f63e151492792`  
		Last Modified: Wed, 17 Nov 2021 02:47:34 GMT  
		Size: 53.7 MB (53669238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad19338e0216949f11a92dd8945b6e22f31f21cf795fc761001c8a74e348415b`  
		Last Modified: Wed, 17 Nov 2021 02:47:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
