## `debian:rc-buggy`

```console
$ docker pull debian@sha256:4c33f8fc1416a053966646f8b5f92bbc12423c10e2b665d0d1a94e872c9c96f2
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:af50f3f71e067ee3abf5fafc35ead712abea35ebbc5a154b144a91203cc87990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54909527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec9a40bdaa18b33b9b16aafdefc8fb007491f6bd39ce5bb7bf0b0f8f5e5bc523`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:46:20 GMT
ADD file:cac9ad9d988141c80929e8c31f4cb388618dac0bbc048d4c5e3b8029c85c576d in / 
# Thu, 22 Jul 2021 00:46:21 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:48:15 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:531fc43e70accbfd0e52721b79cfd564769d6f1b7e64a98e9f670327d4c4820e`  
		Last Modified: Thu, 22 Jul 2021 00:51:36 GMT  
		Size: 54.9 MB (54909299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a60b4905cbef3c3b87b29eb23a8bff62eee38c2d0769009e9feea71a5e62b97`  
		Last Modified: Thu, 22 Jul 2021 00:54:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:8b6caaa31f4e686cdf9d5f0abb7daa30686865a7f30ae4c56474a2cf53a0cc5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52446214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fc7d60a62e6eadefd396e0fe7859788856984ae922b23e8e2b4232fd19e4db6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:51:25 GMT
ADD file:7b9b18b6a1a6deb81eb9bf8638d60de26198ba106aaa757dfb838b264fc90252 in / 
# Thu, 22 Jul 2021 00:51:26 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:55:44 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9de879dbb26d0cc624c499f5907a14117d0f357e4e39699d3208c57d5091b537`  
		Last Modified: Thu, 22 Jul 2021 01:04:16 GMT  
		Size: 52.4 MB (52445986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4113094c4051f4a02484e5cd1254e6fd98d6926c2f79a4e7cb5377ef771fa8`  
		Last Modified: Thu, 22 Jul 2021 01:10:09 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:bbcdcc20257e2909995ddab15d3ea9287dbac5d0c4130a627c56b2d1d9a630db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50112191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed317a31c5faf540db57506547f76e86fa58d0f756fe9d1a84e1f2b965ad61a8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:05:12 GMT
ADD file:dc3a5129f00ffe49d5f2b5c7472bb0e89235fc02cd3f1cc7d27243e371d4a8e9 in / 
# Thu, 22 Jul 2021 02:05:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:09:42 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d81caeed2081307865201ac11c62494bbd309b5efe940cf9cae7a6739c8ca2a0`  
		Last Modified: Thu, 22 Jul 2021 02:18:16 GMT  
		Size: 50.1 MB (50111961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3c170cc3d0c91e284dd12fa49c64223d08a4d0e2ea9d465c988b29cae17415`  
		Last Modified: Thu, 22 Jul 2021 02:24:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d7417d7cc6b012b41f0ba68641ec26ed5552ad7250458eb494037980f56c5f92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53593299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1fc0f9eb027ef13e3bcd008a0e55060f07f6dd48484dc2d46c51814c6e85bc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:46 GMT
ADD file:a3549e948b3f56a447f7f9b8c10f86c1915a2f52c546e1e7891735ee86a647ee in / 
# Thu, 22 Jul 2021 00:40:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:42:33 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:62e8b52de22392fa7c459ae1bacaf43117fdae59adb2ad8b421412ace5a516b1`  
		Last Modified: Thu, 22 Jul 2021 00:47:01 GMT  
		Size: 53.6 MB (53593074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31046105e54924c9954108d10a891c1f5d886066e27caa7532a86cc0ed77c326`  
		Last Modified: Thu, 22 Jul 2021 00:50:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:8de331bf0968c6c750410c6e69dfea77fea650aae83d9c2e3782ee2b236e67e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55915460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd5feeec2f1836c9ab6f074de4bac2095bb9887ccb6bb0ea35f2d20bc066b06`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:35 GMT
ADD file:a05f9816b9e0d809ccdad5c4c30efa7318e22e8cdbe05e2d5311dbe3a25d8e5f in / 
# Thu, 22 Jul 2021 00:40:35 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:42:55 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:92fe8ead237eb68742a0dc7b6d1566536376e794dca6fa5ecebb1d8a469370b1`  
		Last Modified: Thu, 22 Jul 2021 00:47:52 GMT  
		Size: 55.9 MB (55915233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8218811726a095d2e3bbaaa87ac31bbf7b3cb6aefde6588b6dcb2cd96caec8`  
		Last Modified: Thu, 22 Jul 2021 00:51:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:2ede766976a21c690b701a3b4462a7dd804312e4d83518234f8a81696b8d3d17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53162379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e05b86b5a23254e415d2951672c9e1d6ed5a46d26c6e8c76e4fb7378799fafb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:10:12 GMT
ADD file:21823f99ac9631853baf61992ae48f9aaefd9aa14689bdad76945cbe790d4b23 in / 
# Thu, 22 Jul 2021 00:10:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:13:02 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b7674bbd759fec6741d7d94cfebb5e0cf54c599cb2a824313eb96b1d6622a44b`  
		Last Modified: Thu, 22 Jul 2021 00:16:59 GMT  
		Size: 53.2 MB (53162150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d9ec8bb2bb4b71c20d9ebe541ab05f2a48282483fbee7dab700b12fdaad0ee`  
		Last Modified: Thu, 22 Jul 2021 00:21:43 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:618b650726005ebc03856cb8c36807917539485d440d00c7124e57c57d8fe5b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58810947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639ac7f5e749eb75c4418f6fe0deef36098699febf80e77e27f7f90a2894d0c1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:33 GMT
ADD file:d5172916465206276bfc66e1d963768fd3cda811ba961e86fdbc4b49f0a72dfc in / 
# Thu, 22 Jul 2021 00:19:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:23:37 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bb31d3e4dd3826fb7298bcca3375efce01b08c74be37a5494cb4eaccd247d8e9`  
		Last Modified: Thu, 22 Jul 2021 00:28:17 GMT  
		Size: 58.8 MB (58810717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac60841a68e5afde7357fc934f78d4e1329f114ec0830c5d2ca34d35d333cfff`  
		Last Modified: Thu, 22 Jul 2021 00:31:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:d32d9956404febabf42c501b82bfaf2dc45f4d15fded7082e0fd5ebd85b498ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53187558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41d4e7cbfa8ba4dc37bfaff8f26ec7ed6777c6680f05d0ef00e168127d39b30e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:43:01 GMT
ADD file:eb0fa0f991634817ac5af2d4e957d8d14c8fb5a8d501cfeb56949d715ca84f1c in / 
# Thu, 22 Jul 2021 00:43:08 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:45:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:730f0cea2dc4896e7a1a70e4e4e14165f66e42bcd880b7b7242a68c9d2ffa297`  
		Last Modified: Thu, 22 Jul 2021 00:48:31 GMT  
		Size: 53.2 MB (53187330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9667211d52527a935b294cdbcbbb62e609ccd0436ca340c666efdf37dc3d22`  
		Last Modified: Thu, 22 Jul 2021 00:50:36 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
