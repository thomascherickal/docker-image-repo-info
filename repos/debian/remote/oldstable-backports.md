## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:c2bd70523141ab58c901c7b3fdf7585a842a0d693db18648397c84c3b72c40bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:c4d674cb60812aa997f2e2c9fd9d55b53279fad0cd592fd163357d4a975db82d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45369889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83d506d082d18acfa894da73c072d6c40dacec18ba302a421d026cddab168542`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:05:05 GMT
ADD file:d82d5477ad39cb7abe24ce64e83337baf085a09223487876e34f8902d7e959b4 in / 
# Wed, 22 Jul 2020 02:05:06 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:05:11 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2c72f8e54c0498da77a3186087ede3cd0f8c19f98d2f0391c1af097906d684c8`  
		Last Modified: Wed, 22 Jul 2020 02:11:03 GMT  
		Size: 45.4 MB (45369662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efaac8181bd2a0d274a90fec1a03fddb99d6e2a6112a8444e71dd15f7f5bf0c`  
		Last Modified: Wed, 22 Jul 2020 02:11:07 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:4cd9d1930ffd12130a156c62fd12f3cc7bc72fc7a42711996ca0dfdb1f70bdf3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44078517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f86089ed73b78608d2e8066da7695b9668531bc0c3acba371e6fabda2e457a2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:52:44 GMT
ADD file:b25df371e82fe7adce89a094766f6dc098a39d5db27105c588b1bc8772e8ac0a in / 
# Wed, 22 Jul 2020 00:52:45 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:52:52 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3b788099312f5c96a034535c0ddeceb41d0b1271ba8b28315cbced400202d8d8`  
		Last Modified: Wed, 22 Jul 2020 01:00:53 GMT  
		Size: 44.1 MB (44078291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63b8a378f6f36bff20f121afc91fbb9ee022757c8967782ef582709b94bdf92`  
		Last Modified: Wed, 22 Jul 2020 01:01:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:80f66628d0313a840455fe89b4b4dddb481af3276a53d37dc5412b535e17a8a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42107653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:770c22caf102d9da7000549117594aac3ee5ea0f51dd614b07b25949f07cc555`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:25:24 GMT
ADD file:14cc58e8ae9b03746c983cb41d0fd43f0d339cadb578d2e02090071a87edb324 in / 
# Wed, 22 Jul 2020 01:25:31 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:26:26 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eb4312b69f0e4d6f13fab3412235cb22326cfa3fb057f0a62e9d8cb585c19063`  
		Last Modified: Wed, 22 Jul 2020 01:42:16 GMT  
		Size: 42.1 MB (42107427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40ed1914e4748d0cc00aff8d12b1edf61321176e08106f0f72ec8832d4a982`  
		Last Modified: Wed, 22 Jul 2020 01:42:23 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1ab9860741ab88aacf1a758a8e40d1d212884528c068569cfe35346d1666edb9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43169596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b021dc29389068a2ad632474e12385d98a931916b0ba3e7f92fd45b2b9b5a793`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:27 GMT
ADD file:c3e784b1a0fcf338c9ea2e4941098e5301a514012f3a924750f3b0db08153603 in / 
# Wed, 22 Jul 2020 00:41:30 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:41:39 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:41ea194606dcb7fcac3404e4f40fe7ed4b8a22ab9c27f1ad4ebe3b3fb4c9998f`  
		Last Modified: Wed, 22 Jul 2020 00:48:00 GMT  
		Size: 43.2 MB (43169371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27aa998deb60e54bca64139bd92f84b5d72a06f89480fce7cb7350bf17a2f1d8`  
		Last Modified: Wed, 22 Jul 2020 00:48:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:f9499a3a425b02c13d20a8d923cb19a4a24d6940b1b78466d2fe793949fb7927
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46093276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89630fc281e037635cb71a17a0baa0ec6245e195f7285b385dbfea7891087553`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:10:38 GMT
ADD file:b7c7c068cad1cc8a4fa8431babebe8f4099a7c2e540ed4697bf1b0c01e4c1a40 in / 
# Wed, 22 Jul 2020 02:10:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:10:43 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:86642cd6812c35d602060e2afe32a1cc63b7db7aca5448c1b9df26f567f88653`  
		Last Modified: Wed, 22 Jul 2020 02:17:33 GMT  
		Size: 46.1 MB (46093055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad57a298f3e7063b556fa34dae2da64d6b2e1f6ce5e663f3c0dbebf883cdd1e`  
		Last Modified: Wed, 22 Jul 2020 02:17:38 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
