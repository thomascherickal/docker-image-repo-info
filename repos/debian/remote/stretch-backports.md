## `debian:stretch-backports`

```console
$ docker pull debian@sha256:09304525f74f63957d08b2b7534d3fda133d715b48455174cedf62d51080b9f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:1a37eff29ce1dce142e55bc9f2449fc1a1757f72a64fc485a8dffe918895027f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45366949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caf61755edcb6deda91fdb298f7241265b627491b1117224c33000629729c735`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:30:13 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f237ff9ea175532b57ca59290e2c66d270152aa3b76422c5061dfea560272b9f`  
		Last Modified: Thu, 10 Sep 2020 00:37:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d96c6ffd378fd0b55d71f23d8b28f72ffc67b5dcf01bd2194d96b91bf2514f51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44081522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2701cbfc5a515049bfe5235b585dc29cb1aff778adaba765a6494ae0652a375`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:58:16 GMT
ADD file:39312a9e824bd7c6ad3eca3ada9e922d8f7219c51e10047672e9ccab3dadb248 in / 
# Wed, 09 Sep 2020 23:58:18 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:58:28 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:301ffd407a7ebea8722c85a0474f1c621b0785275eef7a32a1ab7b5106a8e762`  
		Last Modified: Thu, 10 Sep 2020 00:06:45 GMT  
		Size: 44.1 MB (44081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da7b2df77b574445a17010dfe1f2c01c71ccee499c0dd6d545696a0463d041a`  
		Last Modified: Thu, 10 Sep 2020 00:06:55 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:30b638abb76f488f44edd17054b0ee33cad8b2cf2088c57d19a51dd9d64d8421
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42111656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f9be08dbe21388f51a774698c6c0472f822131d915431ef74429e179ce1125`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:13:17 GMT
ADD file:3da15ca153ab01cc777bb2a828e1097edc064f49012d96e9b0789cc4cbe9c205 in / 
# Thu, 10 Sep 2020 00:13:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:13:26 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2dc31d01bd52bc4550017dd5cb9e295a7998fbfa6b3ea3f612efb5da666b3600`  
		Last Modified: Thu, 10 Sep 2020 00:21:14 GMT  
		Size: 42.1 MB (42111430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699893cc2f0bd07a525ae37f02f9a75cbf7b69600c9d7fce642ea9c20fe7d65`  
		Last Modified: Thu, 10 Sep 2020 00:21:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:643ba83668b4a86bb8fdf122f4854198e606001e70d29a4c9c72583dfab31ddf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43171923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797329518abe286c94b07d53bb66c50e340ea93abd880fa9d5df316e0e3b06b5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:23 GMT
ADD file:f74bb8d38ef70a022988428f254630d1f424ed9a3b957687b0cd0f85b9d49e29 in / 
# Wed, 09 Sep 2020 23:54:25 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:54:37 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3b396f138ad78ffceac749b105c676dce568fa15a7b9f2273c2ee13ba023cea1`  
		Last Modified: Thu, 10 Sep 2020 00:01:33 GMT  
		Size: 43.2 MB (43171697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c661db5c30a810a5f9502cf9df11a7a66fb9a4a6ed50e2e9cdda2cebf30547`  
		Last Modified: Thu, 10 Sep 2020 00:01:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:0ca1e041768566f9c590494c8ba3c4792ff44c9a6469c797b16c47d702d7724b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46087005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ae2c16fbe806dc3399cce594706798cf98dd27f2e63a055be62a61c2bb25a9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:43:30 GMT
ADD file:615d959fea19ddc0e0fd27a59a77c1da8526b37da0b65bae0bfc4aac68c83ad4 in / 
# Wed, 09 Sep 2020 23:43:30 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:43:35 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5147f8567709ad49d5f034aa307bd29bdbbe40bcf438c67f4bc82655742c25c1`  
		Last Modified: Wed, 09 Sep 2020 23:48:59 GMT  
		Size: 46.1 MB (46086780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbf396e5750dd32115852e2fafcf8592af19f9a1becd38ed6b9590f1b29e01d`  
		Last Modified: Wed, 09 Sep 2020 23:49:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
