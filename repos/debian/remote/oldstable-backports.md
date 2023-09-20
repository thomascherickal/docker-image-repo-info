## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:55b9fd74358aac7119ea28507b3ec2feca8652a3ab3f02e18f617924edd68c13
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:ef429668170f94b752556285d9b98d453dd69c2ca7fc8955948face61eecdd4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55056490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62020abdb37310ccbb46a2b5fe0580d129ee9b344e3008eaf824458b0fcaad13`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:22:05 GMT
ADD file:52cff30f892389172481cc0359bde2ed2dd4acf4a189dd57c1f56f407d9b3d7f in / 
# Thu, 07 Sep 2023 00:22:06 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:22:10 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9d16c0ac7be786ecfb9fb46c48e4dcdcc40afa63d97c1904fb6088e23940309d`  
		Last Modified: Thu, 07 Sep 2023 00:27:35 GMT  
		Size: 55.1 MB (55056266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25449fc52443cf7c7eb0db7ae3189bb0f26571cc80f751cf106cca2908cf538`  
		Last Modified: Thu, 07 Sep 2023 00:27:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:4386958b015f7e44bd738ec9710928c4faeddd65d50fe1816273ca03abb9bb68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52558398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d825a2d2e14dc9c06d92736da5da3ba08f9e249ac0c03e784080641e592eb6fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:50:35 GMT
ADD file:6585afdc8b7840bcbfa96fcb0bf0d7d7e9eb5539dd1cec70e5ee6f31209ad3d3 in / 
# Wed, 20 Sep 2023 00:50:36 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:50:40 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ea4d6080a0290f592c439c3add7fef2662b6e325c704d049e34f299626e409dd`  
		Last Modified: Wed, 20 Sep 2023 00:56:03 GMT  
		Size: 52.6 MB (52558171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209b7809d4853aa26fd899302544e9e1180418b029b1ce42bd978582e9dbf05`  
		Last Modified: Wed, 20 Sep 2023 00:56:12 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:523809a34b54a8de51cb96e2e23d9ebd9b54f541c62bd4c20f9131e30a2adcff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50219432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d23ee51b4857b0193ae07b791f9074065241362f47c1ec8293e079b1e5173`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:59:08 GMT
ADD file:dde253d9c1302aa0f98aa4e009d679edc1477ec26433508aec5adbe7194529e5 in / 
# Thu, 07 Sep 2023 00:59:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:59:11 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:995a6f506d1800e9da0998564c6bf44de76a9ac7b9ef77facfd8f5f5983e3703`  
		Last Modified: Thu, 07 Sep 2023 01:04:46 GMT  
		Size: 50.2 MB (50219209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed31519919b6228e52c0501ab65d120fc1d9eaa851e88c35e1950f01c8fd9734`  
		Last Modified: Thu, 07 Sep 2023 01:04:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c0015d6f7e307abf5e8dbbc0e59256b24225e5a2519b6027d45a10239c6c119a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53705106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d856472b558fc55d617578865a34db42d1fb4bfc86510e7a6a8e9958f6435a3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:02 GMT
ADD file:d17683ba7f6b9175b6b7355c2a92df3ac32d932885900024a59637e9e84daed8 in / 
# Wed, 20 Sep 2023 02:45:02 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:45:05 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0250f3c681d4d2407c6615b27e9cef12ae5c5df4efb11d3c6073565ea79cd584`  
		Last Modified: Wed, 20 Sep 2023 02:49:35 GMT  
		Size: 53.7 MB (53704883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d21f03d83f060d7bd6a6596a5f7cdde8753dd313babc062d554d186fd03e07`  
		Last Modified: Wed, 20 Sep 2023 02:49:43 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:4ba1e830424d3a22ddde701827c75cace333d24ebc11a12962d85387bcae17cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56040710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01b63c27a3887663d71b353e811a74bf4cf99096ed1b86d514f781a8ca6ea2bd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:43:15 GMT
ADD file:4972d10c6107fd20bf98c1c94a441e2cb3d14a625feb9e293d0b7527d3c8efbf in / 
# Wed, 20 Sep 2023 00:43:16 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:43:19 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:73d05fbd9bfd3b656f84a6e1bc2e910f22de1d965198a98739ccd97ffb57a9cb`  
		Last Modified: Wed, 20 Sep 2023 00:49:26 GMT  
		Size: 56.0 MB (56040484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508dc8e0165a6fa72f96bd91e0c60ed4728c023d52bc243d580fe6177926b06`  
		Last Modified: Wed, 20 Sep 2023 00:49:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:6d9a9a5685c9c2b118859c74005a6dbc36b4c4c212670e197fa9225076653da0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53271806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c0daec3f99022821762b122540811baf035ca3bd95f6c201cceae7c07e1f8f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 03:11:50 GMT
ADD file:b66228ed1d56adafcf09e54a7851e635c035f251b00b1b0d21a0abaa88ecbf07 in / 
# Wed, 20 Sep 2023 03:11:55 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:12:10 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a544bd17008b1d9674e58ea820849b847656ef432805f1935b82a7322697869f`  
		Last Modified: Wed, 20 Sep 2023 03:23:10 GMT  
		Size: 53.3 MB (53271579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb732a0ea07be713dfd4b4a74f744ab03dca30dade7566c99c957621e4fd56f`  
		Last Modified: Wed, 20 Sep 2023 03:23:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:93c0759ecec4d18a0fb20524d6b7855eb6ae8be567e5e2ce93186143ecb938a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58928346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad90ecb4e4702b0db3da8d65f6faf2f3d1f183a13e0c814b152fe57b0aa49c7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:18:22 GMT
ADD file:e66bcde662505500cd1c9ac76d9ae76cfad59f8cb57b4951c4bf0aaf1c951b2e in / 
# Thu, 07 Sep 2023 00:18:26 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:18:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3e4b9a8f54cdd852a98f3fc55d957ab3de7d2430e8ac65164b7b0423bd976387`  
		Last Modified: Thu, 07 Sep 2023 00:24:51 GMT  
		Size: 58.9 MB (58928121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b993fdc85c91c6d40b687e1ff315e05758791494fe0a669a14a8e6689582b93a`  
		Last Modified: Thu, 07 Sep 2023 00:25:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:c8dab8cadc970bb49ccf10d4c9aeb77b0b1ff0fd529361512d9a284ab9415449
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53291009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277eca3e137e8ce45e36aef3ec6074f26f1da1d3a1bd094baae86c9302efec2c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:55:06 GMT
ADD file:70ff196e59910a6b186b452eceb08d0c1512341259f133883037b5a812790449 in / 
# Wed, 20 Sep 2023 02:55:13 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:55:20 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3f4df5cb857850953aef5626bd4096d5e588a823a5d9609a0e147b118c9a539e`  
		Last Modified: Wed, 20 Sep 2023 03:00:37 GMT  
		Size: 53.3 MB (53290785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd46ce1d19cb915e216266c3c1042d60d099d39b16c8e34477dc62a0818686`  
		Last Modified: Wed, 20 Sep 2023 03:00:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
