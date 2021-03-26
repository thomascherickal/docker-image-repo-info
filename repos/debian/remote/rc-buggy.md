## `debian:rc-buggy`

```console
$ docker pull debian@sha256:848c984e2e3bcec03d0baa77437132a4d16cbf3cf0c75a917ee3d56d9ec4d6e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull debian@sha256:772d670d69724ffdc6caa3116af46dcfcd141a5d60272c79642cc06985093ef4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54840756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f04fc7094a70829d5492240c6600be05f6345d6e8052b56943978ea69573d7ae`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:21:52 GMT
ADD file:719f8702f6aa56e8ad69f574e924fdf062e8fdc72584f70aaac387be5e1d4a51 in / 
# Fri, 12 Mar 2021 02:21:53 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:23:37 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:78c7a03f25ec710f7b6b9ccc0ee40eb1871016252eea6df272c68389f18d30a5`  
		Last Modified: Fri, 12 Mar 2021 02:28:37 GMT  
		Size: 54.8 MB (54840531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ba105463ef9c3712f1cbac075e1d61bef0d5f438f41f5969e7c13a3cc49b2`  
		Last Modified: Fri, 12 Mar 2021 02:32:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:bf170c96f450fb286e07e9277fe04dfe2387ffac56a3e48af6a599a30c6a778e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52402653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fca722d7b5ee88c688aaa898de369e6f63ff5a5d2b77046e96ebb50a549d28b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:54:14 GMT
ADD file:ac1ac9f39520995697d7545a4221ddb94e841eedef2eaa8bfc265b3840c9d873 in / 
# Fri, 26 Mar 2021 07:54:16 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 07:57:48 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b6ade6f33ef6b8c4fc72e7adf3004838c72714ea31573c675126f6144bbc650e`  
		Last Modified: Fri, 26 Mar 2021 08:02:48 GMT  
		Size: 52.4 MB (52402425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a943d58730c67d8b820d25a7ca5ca823915569c9b313df7e41c14245e3b7582`  
		Last Modified: Fri, 26 Mar 2021 08:06:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:1d47557880dde003e5f4cd60c4d45dff37f516deb330dc15992c3156cbdc6ee3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50045793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f1c51a507721498cc4b91e11487486e26d0ce3049dd71b6b5ad34a4b0597474`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:03:15 GMT
ADD file:14dd8de951fe825db7d388033d6936d3035ea22c36f61cd84e564b5c97ae4fb6 in / 
# Fri, 12 Mar 2021 02:03:18 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:07:51 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d53db477f7b952a423ea709246666b7c318b3cced3843682efc6d4a208dea579`  
		Last Modified: Fri, 12 Mar 2021 02:12:47 GMT  
		Size: 50.0 MB (50045565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afd11a97f153cf2373460fb55018db1949794000f71f01315fc9a5e63e6ae14`  
		Last Modified: Fri, 12 Mar 2021 02:16:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8d41dd306b71109a1d6718d8720787fe167efa572b155d7ad5397841edacfb25
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53528972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92d0118c5bff73328ae674fd6cf4a862cf3ffa839d745f1753fe9bfbcb57625d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:55:07 GMT
ADD file:e98b46fa08e28b488d04d4429e536292413d7b6dfbd8a34310c44a6b65b421e7 in / 
# Fri, 12 Mar 2021 01:55:15 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 01:59:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:443483bbe5c8ae014cc3cb8df57a0b708d2b55560844a100ea84ee50c9b1736d`  
		Last Modified: Fri, 12 Mar 2021 02:02:40 GMT  
		Size: 53.5 MB (53528745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bb454115f1315abd939b77b5532b71f2693cd8f8e9b91529076561a7929225`  
		Last Modified: Fri, 12 Mar 2021 02:05:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:61b618239e46d1ab50d9026ee3d759f275bd0fe553cbc73c529ded64e16fe402
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55863433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8991dda9ecdc29a45468bf588a4cc7fc725d5bf2ad71ffda235f361151a197e6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:45:58 GMT
ADD file:f2f05e5770523445c3d58c38661c24400d3d13e8d89e5e8b361fe9b063862930 in / 
# Fri, 12 Mar 2021 01:45:58 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 01:48:12 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1d51db899b128072895ed240852af0ccc606db1f5e0eb5b88ceccc9b8bbd2876`  
		Last Modified: Fri, 12 Mar 2021 01:55:02 GMT  
		Size: 55.9 MB (55863208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8309ec56246eda69d505f961b9c478f4aebff27b509a0a174afa1e69773901b0`  
		Last Modified: Fri, 12 Mar 2021 01:59:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:52d7073108d0cb2a135148a21ba300060ec180f10effa96215b3a651571702c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53127051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:237ef90cea5bfe70607d8ecf748c6e571c90acfea9641c863775c13c4c3003dc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 08:10:22 GMT
ADD file:45a8dd112a282d4aa23c7808fe9a53a90aed8669a8c0886cbd1b014e6f666e5c in / 
# Fri, 26 Mar 2021 08:10:23 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 08:13:14 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:dc0d626a86c29f3dd61b7699812357277c6ad4db66ed29b70e541593f9a413f7`  
		Last Modified: Fri, 26 Mar 2021 08:17:18 GMT  
		Size: 53.1 MB (53126824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8c3448dd2586560dfec757704696c032e665bde4f2644d1df7904601768d3b`  
		Last Modified: Fri, 26 Mar 2021 08:22:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:37ebfe449dd987a43dabc27b8258419e9013b7e9a2ac627dcca96179ee195994
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58754070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888de08ed55a803a1e3cc8491bc6f013525fa4762d35f036b91765e0cb38434d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:33:07 GMT
ADD file:976d560bd7f7860fcfb64f49aa1043a087bc71ae5099f0cb06a93ac6051ac5df in / 
# Fri, 12 Mar 2021 02:33:25 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:37:55 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:45911da2c88811278c7ef0cc34bf94d713837727d8059f205da3332e2aba2766`  
		Last Modified: Fri, 12 Mar 2021 02:47:13 GMT  
		Size: 58.8 MB (58753842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafda66d0fcdc1c9e09dfab633d8d6f3fd713b4a4b3bf0c7fa89078dd24505cf`  
		Last Modified: Fri, 12 Mar 2021 02:56:47 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:bb1f735f4ec1f5c5ee69d2b2747ef6d0e5abbb5974b91c793bbc8ecddcf9ec26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53116598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e95b85b4ee280a4e89e3ad75d6e56dcc63d75d5a236e994dbbf66941379845a9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:21 GMT
ADD file:0ca8df72ab8a25212bc85ec53930c9285a0c63ea73409a2e42e8749af8d051be in / 
# Fri, 12 Mar 2021 01:46:27 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 01:48:56 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ae111c7645dfe78b7684eb4252c76f987ecccd3b0e2f8bf675e007362fec66fe`  
		Last Modified: Fri, 12 Mar 2021 01:50:46 GMT  
		Size: 53.1 MB (53116371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d492c42c9788e52463c54b86b66e84c737552832515471b056f01ea372deea4d`  
		Last Modified: Fri, 12 Mar 2021 01:52:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
