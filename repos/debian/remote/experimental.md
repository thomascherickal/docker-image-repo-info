## `debian:experimental`

```console
$ docker pull debian@sha256:463a9ac6dfda396076ac9022cf24e425c0036d57cbcbb39d6d3cd817a3e37d4a
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
$ docker pull debian@sha256:0617bd38dcd8501d811b068b5be53cdad92f600c1c6ded5e8c5b9c82be3209e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53226562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486a376616eb383a97852689617ff514aa16fc9f7d82c1b465f21a9573085e99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:22:14 GMT
ADD file:b859e5fcfd3a7197bd32bce8a01edec8ed645ccd01bd5d277fe37eb193fa0fc1 in / 
# Tue, 12 Jul 2022 01:22:15 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:22:28 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5171e606d7acf20fe0ce394fd5c9a115a61b39c2305b47fbad26a83be0bc3afa`  
		Last Modified: Tue, 12 Jul 2022 01:28:04 GMT  
		Size: 53.2 MB (53226341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e703dae63cfa425761851b769df1c0a7ac8758947d438c7fd114f9ff5c2e52e9`  
		Last Modified: Tue, 12 Jul 2022 01:28:28 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:65bda137ef63b6b3b342e7c9cb06b77a4f717221fddbf5842a778f5cb8ecbb2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52021628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bf43d48b8acb770ae16c12f63dc174ed8451a2bbf51cdf58f0945107a3345a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:51:50 GMT
ADD file:8165c0d978757c272b0fc9aab3bf8bc8644579a857290a6ba3d25f5e06be2ad4 in / 
# Tue, 02 Aug 2022 00:51:50 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:52:07 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c32afc4cc9c9df6d376376afbae71bc1e87837dd8838c5d55f5854ba7298b657`  
		Last Modified: Tue, 02 Aug 2022 01:01:30 GMT  
		Size: 52.0 MB (52021404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13804901e30c4db3bf34c853bc1b62a7f18ab26005b2da85a952728ef852af2c`  
		Last Modified: Tue, 02 Aug 2022 01:02:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:dbc5fb5ba3f3cfb4b7738419e7dc8ca9c6dbfe59d0f76f144223c4e5fa320b8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48767835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e676526688a13abb7fb464eb77acac18731e9dfc9341a13dc17a4b9aeb542b6b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:05:37 GMT
ADD file:37af7e1809e2a0817725585525744a092f84ed27af17d736f77f96af05205ccf in / 
# Tue, 12 Jul 2022 01:05:38 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:06:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:22bb7ec0f68d05282d548a6a9c1ae9a71eccd98fd5e2eddafe630ecd5d4d4f58`  
		Last Modified: Tue, 12 Jul 2022 01:19:20 GMT  
		Size: 48.8 MB (48767613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b2d5e08cbf65c7d3a06f8758f28f9cfece6b2f6d17a5c1f68911004cac42c9`  
		Last Modified: Tue, 12 Jul 2022 01:19:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:58e8138be5496b8e39af0d52a9560cb08b32ea8408971b0d687c37e81d337eae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53312003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9881d82d4e8ede46b1c4a370dffaa02c73b4e485e347e2bceb4c97cfa162b26`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:43 GMT
ADD file:f319e3ad56cdacf4f559c33e21c65bc34192203c7cfe561c49951febe8d41d11 in / 
# Tue, 02 Aug 2022 00:42:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:42:59 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d7f89fc086c7d917b11f43154b1526ea2314922b905525b6bd85dcd4b7ad7e96`  
		Last Modified: Tue, 02 Aug 2022 00:50:22 GMT  
		Size: 53.3 MB (53311783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2758a8c5115b90983ff91e9450cf9b37718bc7dd5da83f326213a388a9526`  
		Last Modified: Tue, 02 Aug 2022 00:50:52 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:9c6767364508033bf234cf39b17b6eef7285da5f9a70091ebba1620033b1d277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54195289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9542ed6f00ef909f4d84470f0a8f4cd531f9336da9b31ef20d1e76173bdc5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:33 GMT
ADD file:86aa5ea5e610e7d9bd402025a337e0f305b103598be63b78b6b0cdea7a3df4de in / 
# Tue, 02 Aug 2022 00:41:34 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:41:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5699b5f3fd16f897714b4784f589776f740c6550b1714d3050d6370b669db263`  
		Last Modified: Tue, 02 Aug 2022 00:49:25 GMT  
		Size: 54.2 MB (54195065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0841e5987f50cdeaf45bf3836fa418307c90a4e91ac439e2fa3451c95b330918`  
		Last Modified: Tue, 02 Aug 2022 00:50:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:2467637aae94e7abece607dffe9e531ff8e6fe38f95cb5bdc3122d975b88fc79
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52346427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b4c7cad37b89a168270577a1f7e7f489bb88b74d5f9764383bf65aabfe0827`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:47:36 GMT
ADD file:feed10c6715a183ccdc9f46ba4cc94249d4b2074e13fe1b6d2ad8225e7d3dec1 in / 
# Tue, 12 Jul 2022 04:47:42 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:48:19 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:17f25a9f849afa7fa4747c7fb4df563f0a135a4ce73aa1e98b4f3b5580c358f1`  
		Last Modified: Tue, 12 Jul 2022 04:58:36 GMT  
		Size: 52.3 MB (52346203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba2fe012dea5d8eab5649c500fccbc51efc23e8841685bc72e0a13cd3024a63`  
		Last Modified: Tue, 12 Jul 2022 04:59:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:c8a5bdcfca6fee4a184cecbe6b35335f4e4451bafb4d587d0df580ef274aec49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57441689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11ed9d6235dd871fa1c242ebee3b156bb0e510f5e5ed6bdcb2f8c44bf5415e14`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:30:03 GMT
ADD file:e682e7df06e8d44ac1f07bb76baae4ee7539c3668b05c947733d8ebc5ee63615 in / 
# Tue, 12 Jul 2022 01:30:08 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:30:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f37854ad4016381ff034d6c892edbcb45ff9b4ca51638673ca7781fabf94f110`  
		Last Modified: Tue, 12 Jul 2022 01:45:27 GMT  
		Size: 57.4 MB (57441465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77b27e9b4b4421d825080d7e4dd4fc5ac9482fc3e57b5b49cc6ed6064eeb369`  
		Last Modified: Tue, 12 Jul 2022 01:46:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:dc897e670cbaefc2e4349a9c47bf6ca09fc2873d9cedcc45eb7fa91784b104cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49440941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04a2bff9549bb8e8fc889c0b753fbd5a0a0a45f8b6a9a3de5264d4fe75e40200`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:14:32 GMT
ADD file:c3d46383f0f1686d37d58c4c8b44081da09ee5ea4c5d93f86cca7b7bf93aa8f4 in / 
# Tue, 12 Jul 2022 01:14:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:18:08 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5ffe8ddf58d9cb4f3db87b67b24205dbca09c9ec9f4661416e7d7d627ccb2df5`  
		Last Modified: Tue, 12 Jul 2022 01:32:52 GMT  
		Size: 49.4 MB (49440713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe8a4e5dd7f24a326c6f4e765419cbf14f4990ceab9dd2d8e3bc59291c50c8`  
		Last Modified: Tue, 12 Jul 2022 01:35:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:2cf3bb5edcdadca734a6b4cbdd3512205941b22d6f79ede0aad35e46219c3579
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51734886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a25d77266bb510f6a354a417d2426e60d538f5f05f61e1e31267bc62cbe9c64`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:44:54 GMT
ADD file:984d42e0d8c3e13cf8d8ee6608f0302c63c5b967b172fdcf3761d14a4b52a4b9 in / 
# Tue, 02 Aug 2022 00:44:57 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:45:12 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b0185da9188245470949775bd4011291c882eedfed309ae9f441a1037dcf027d`  
		Last Modified: Tue, 02 Aug 2022 00:51:18 GMT  
		Size: 51.7 MB (51734667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4138c8d0e1ae99014aac269457329e461183d106799474d741363678a97449f`  
		Last Modified: Tue, 02 Aug 2022 00:51:35 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
