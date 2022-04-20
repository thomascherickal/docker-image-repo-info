## `debian:experimental`

```console
$ docker pull debian@sha256:99cb72c3772e3f2f45e2dfdfd6513e34be838001fd3dcf80f2591c3227281c10
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

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:220bd5d9a869e9c16f5e40369d4d95f848deb3629bdcd830ce7b245dfd558541
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.1 MB (56112901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baeded9577302da4d155448d989777fbbd01564a09c102e50529f25a71cc5b8f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:55 GMT
ADD file:b8f07060f9d2d7f5c4db9947fd089591ea261222b369890ff85325ec74bc0a6c in / 
# Wed, 20 Apr 2022 04:45:55 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:46:08 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7c26de214b349330f4067f62eaf7fbc9c2e817d82821b54e517e1456eedf3030`  
		Last Modified: Wed, 20 Apr 2022 04:53:29 GMT  
		Size: 56.1 MB (56112682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1ad2473963dd6a11702bae6dd1105ba15fa377ce0ac90a6dc700e73c1089a`  
		Last Modified: Wed, 20 Apr 2022 04:53:53 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:44c6434d93ebb2496ebe96fb272c77d5a609dc0ad2d1907c81700589e296fb51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53518731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b2ea52dd05e175b2e7c3dede5320555657e98a27752d33f14f0c405d871353`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:24:14 GMT
ADD file:d59b07addbc058dbb2e308592be3cdab758f37e2b392931b9f1cfea1a3a038e6 in / 
# Wed, 20 Apr 2022 07:24:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:24:51 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:cbf05feef61225dcf4d5af2c7d07b77a5fb04c7158b3585c00e9c665a058ee9d`  
		Last Modified: Wed, 20 Apr 2022 07:42:28 GMT  
		Size: 53.5 MB (53518510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1761de9a86b52c467167e6b16adaabe5d91996db6373998306ec2d40567ef2`  
		Last Modified: Wed, 20 Apr 2022 07:43:09 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:21a33ab43372dffc9b45615b42b85ce44a0bbb880b3a7bc7bd9c1a69348f7eb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50813562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5e8922419bfca49748a0057d97ada05bf46e97203b753860d263f74faa690a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:26:03 GMT
ADD file:bb90352585198bea90f2bd0d7964e8517e01731e7c955f66ceedd059fa9ba98f in / 
# Tue, 29 Mar 2022 02:26:04 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:26:37 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b605358dcc0a53886bb25a6e929d6a2d7e4a45660e7d8dbcae9cc0b75ad566fb`  
		Last Modified: Tue, 29 Mar 2022 02:43:12 GMT  
		Size: 50.8 MB (50813338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077b8e9194028fd3aa880694b3e4ac70fab3336f2c48ff38ed7dcc305def53af`  
		Last Modified: Tue, 29 Mar 2022 02:43:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6a2de964a9853b6cd0bb86c9d4b131d6eb91de19718c82f94be97b13bccd6db9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55064029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13bf1fdf8a672da09c712249542936165a2606d4337a9a7ce95bd052f890e68`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:32:09 GMT
ADD file:ecf4c1717eb6fdd76f39aa7c85e910a5b33b82a012a3115872223977e906fc6b in / 
# Wed, 20 Apr 2022 04:32:09 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:32:24 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2b3f6be4af088219c3879fb497cd5051ae20697284c5fbf8f47d4d9f017ba3c2`  
		Last Modified: Wed, 20 Apr 2022 04:41:09 GMT  
		Size: 55.1 MB (55063807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef30381bc5727e5e206a346f30d3d3d0fc4f4adc0d9567fd094b50bf1e419ca`  
		Last Modified: Wed, 20 Apr 2022 04:41:35 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:38ee325a93ca8631ea38b37bc9e461a77158c8289084636a61b773657011091b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57154205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a0973af1d13f231eca19c39345a629d643a71acbb21da9e22901e20309ebf0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:40:52 GMT
ADD file:76ce7950d3083a262cf5a8a5350e77e81af33edd5696e7bea672c6b56dfba430 in / 
# Wed, 20 Apr 2022 07:40:52 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:41:08 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1b03b8c90a9f4d2a5ce30d33ca3da78514bfc07dbf09d69b25fffd10d5626a40`  
		Last Modified: Wed, 20 Apr 2022 07:50:24 GMT  
		Size: 57.2 MB (57153982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e73fd3a47c092cabc6a0c15e8d36da2a6f5ef49c63065770f4b7e3acef9cd9`  
		Last Modified: Wed, 20 Apr 2022 07:50:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:380732e2f87214c28dc3c99bcef41b4a3b79975681bfb04fe37b414e7d374fe0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54453695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ead74b7d8a28f3208a7a6a89d4e79b34e267a0a49f7754baa33267ed57a75a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:48:39 GMT
ADD file:1f36bf26ba6ed5898744d070089c9800f3701bbe25ca8e98ba248a56b990ac09 in / 
# Tue, 29 Mar 2022 07:48:43 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:49:26 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e7de11e455a9a72d18dbadb02f9098da749f18656d04d5f21c6fbb1ea7ecbfb9`  
		Last Modified: Tue, 29 Mar 2022 08:00:01 GMT  
		Size: 54.5 MB (54453472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad296dfca336d4fc2f7f9dae99c7ee263e1a5e1d9400df740ad175173f34666b`  
		Last Modified: Tue, 29 Mar 2022 08:00:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:2e30526cb6200e9c25e02b5bb9c5f821263ca32585054b0bf126a8fe9bb7ad32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60558196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d3da83de7fb6dae25272dae46a91d7719f8bac376b85404c6242a8acd2f1d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:52:14 GMT
ADD file:66e1a3778c3b5bd2a8d17600540923d83a26fc3c9aaa8a9fb3df562018ddf467 in / 
# Wed, 20 Apr 2022 09:52:21 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:52:55 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b0c49142451cdb4390822a432aca8fd4b80b2d7e389807dbe684df7dccc369ab`  
		Last Modified: Wed, 20 Apr 2022 10:02:03 GMT  
		Size: 60.6 MB (60557977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728e1d0b4de36d3b411e42e002418dae405952cdf11099094206f18cc21f5515`  
		Last Modified: Wed, 20 Apr 2022 10:02:38 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:a1cead4d44ed77c5662eac9f2429556006120420caba2d19a63ec196fc62a185
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51757584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3dda1884db97d35d90d8cc9d6e29762b5d5a1efaa65abe6947b0ed8470c295`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 00:19:42 GMT
ADD file:eb73ccec6d534b35c3f0725251b8917d96bcd87d77d960d0a879ca91d2530a47 in / 
# Wed, 20 Apr 2022 00:19:44 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 00:23:27 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:62d036327287ffa181f78db1cedfa9a2d2ddc4c54f3c3838d75dae32e11ff1b1`  
		Last Modified: Wed, 20 Apr 2022 00:38:38 GMT  
		Size: 51.8 MB (51757356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6440a805ff86b05ccf55572b7ebe62afdf80683fe40032330d06f9f2896e63`  
		Last Modified: Wed, 20 Apr 2022 00:41:41 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:d69ea7db5f051c494d707dd5de6c8e8689acb9fe066d398b2dac3080aa0086ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54331214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb28da9e72d4ec20b94114bdf94421364a665854462661419878eb038003d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:45:08 GMT
ADD file:c6ea51fdbfa2c4af7547b6b1dc6f96d047344c44c7918374ad035c3d804bc0d0 in / 
# Wed, 20 Apr 2022 08:45:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 08:45:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1aa7bce33c54b3eca1469f66058926ebda6d4300fba1951826d8344a4735d337`  
		Last Modified: Wed, 20 Apr 2022 08:52:43 GMT  
		Size: 54.3 MB (54330991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f76843361d0f15c43fec6f84d6f45279e0f92ec42851634eae80c57682cea0b`  
		Last Modified: Wed, 20 Apr 2022 08:53:04 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
