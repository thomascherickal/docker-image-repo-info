## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:3c88f3b4057de79a71da88edb16adade646f6499a46b59858d28578bf61d0b6d
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
$ docker pull debian@sha256:578f70d71b4bd4949cc4c7dd99af6ff97839ba650efd8ec82cb228a84d2d08c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50440794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df1b4b3ba4cda158dce58bd833769595a5ec4e8ec0225a9c8e0196857fefe0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:43 GMT
ADD file:e67a2bb3260496f108614926097424892142a0a3a6921b69cbaed881534c0fe0 in / 
# Tue, 12 Jul 2022 01:20:44 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:20:48 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d8cdb5a0c4ab6682f7cc479b884faadfd33f793e1c8afe72183d3e9da4737d45`  
		Last Modified: Tue, 12 Jul 2022 01:25:43 GMT  
		Size: 50.4 MB (50440566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82adcdd8dfdbea303c8d7ef274ad03aa3b4ed9816c0be30b7d61285a4666bee`  
		Last Modified: Tue, 12 Jul 2022 01:25:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d8610af371632729c53c49d8a4a3df19e237924eb59d22b93b5c63f40725cad9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48160770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fece7754ded2689e21cc737067fcea66895fe826fafd16dc614c61faa1fc404`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:52:08 GMT
ADD file:c548c4d5c56882a23816d6daf3fecf810930a517c6c595d0e3f74a96c9dee434 in / 
# Tue, 12 Jul 2022 00:52:09 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:52:21 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:219f68772cc028ce2582e6e602379a0b22760bf798aea67e7d34e2b900c3be0c`  
		Last Modified: Tue, 12 Jul 2022 01:05:19 GMT  
		Size: 48.2 MB (48160543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf08d463d987066c84111d9ecdf9588ae789352c665f656a2ad916d340dfd03`  
		Last Modified: Tue, 12 Jul 2022 01:05:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a1c639eca73a4dc3634f903fabb09f191ff0a6bc782869419b27316a4ec5b68c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1784988d8c9390b6dc8b0ab2edf83c0ee1378999fa9a30f6853e8bb6ca9bff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:01:32 GMT
ADD file:904613613b3cb368ec9c98cc6533d72ae06b49be8e2236afbc541590c539d34e in / 
# Tue, 12 Jul 2022 01:01:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:01:45 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3751859e53de0d9630f0aea71da948710e1ce88a89879733ef05207cfd7b0373`  
		Last Modified: Tue, 12 Jul 2022 01:14:46 GMT  
		Size: 45.9 MB (45915491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daed964e414fc95be565ca5842d01d0144999bca42de140f95512f3377b4d11`  
		Last Modified: Tue, 12 Jul 2022 01:14:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:58fc8c3fed5baf42b9cd0eede93c7781f4accce5ab47b2342bdb62e374fd235f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:942373d930548dc66c6a52a511c2ddf1018c3aa13c0274a730ae5e0812204423`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:14 GMT
ADD file:d44e3485a1d35f776fb5bc1a9d0fe0aa82f05252f6797fd603393f82ebaa7072 in / 
# Tue, 12 Jul 2022 00:41:15 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:41:21 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:04a0dbfdc60816cff83e8a5a8c741bb057cab6ad6f67ff70824bcf973dbb84bb`  
		Last Modified: Tue, 12 Jul 2022 00:47:37 GMT  
		Size: 49.2 MB (49228925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a71085271a6418455625df4ad697d0c590c6217a675c02f666c4416c2ddf4e`  
		Last Modified: Tue, 12 Jul 2022 00:47:48 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:bdac90928145cf2a991e76a778c70d0a62e5de8ed6e6c69b2ae18f1c132612fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51204233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d08d7fab9a215f14a553dc0d7094a112350db546d508c89bf280a91a3d3a3aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:07 GMT
ADD file:9bf85d9565a376f855995ef65d6714d83ddf3ab0bbb1987b484e8dc3518e078b in / 
# Tue, 12 Jul 2022 00:40:08 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:40:13 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5120b98fe4ffa160b64a47d9c28e92f5f98cfcb24ace97cda5b6a5406fd4c0be`  
		Last Modified: Tue, 12 Jul 2022 00:46:37 GMT  
		Size: 51.2 MB (51204011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce7a957163631c56f3e979193cbbf8d25f6218b5c916e0d7acc70b78caa995c`  
		Last Modified: Tue, 12 Jul 2022 00:46:48 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:ffa1b8b7898906cef4dd332ef875fa5068563d84e677cb2095134e84678722e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49073349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301ebb5cd0ed14e4d5556d75b90db913ac112dc8930b1d9d994f89d1c02fa2c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:42:45 GMT
ADD file:a14ea85307b9b9e93b1b3e35a03ebe2c6cf7ec6942cbf850732803bc2d7dd24b in / 
# Tue, 12 Jul 2022 04:42:51 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:43:04 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:497f43dfda4cd8c3e2bf7e1343c3a7b840f348b91e660488cd9d56cd2d179543`  
		Last Modified: Tue, 12 Jul 2022 04:53:47 GMT  
		Size: 49.1 MB (49073122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfdf92d3971c4959e9f4318001aa3871bae651687ce20482ec36249c43b0b40`  
		Last Modified: Tue, 12 Jul 2022 04:53:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:3647c9bbe574c11cc4cf8ec0a86c6682f1171bba8735d006912ceb9424d873f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54177319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e4a5a3917c565539d0f71f050d4cfcb7748535570082b2d792ef6ead6c25e00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:26:41 GMT
ADD file:1b516c064cfcd9c7e7a3c10601803a8d2f767d7689a53ad90a27e588c091c826 in / 
# Tue, 12 Jul 2022 01:26:45 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:26:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7060ba5c5f34d79ac616a9711d022d626f6c129bc55b7fe5a5566bb711d25d7d`  
		Last Modified: Tue, 12 Jul 2022 01:39:06 GMT  
		Size: 54.2 MB (54177092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183b292d92e8f5251844384c120a75e1452dd2dd50c621ef1f2b28142c8fbe28`  
		Last Modified: Tue, 12 Jul 2022 01:39:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:f3f3461125cad05d64b872bdd148764bd2a5249286fc79142e41f350bdb5cb1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49007206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:776cc1762f3d5bb46967fcaced6a5fb03a49669996817c1b58df18f8a111bba3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:45:09 GMT
ADD file:1ef8c265d400d0a107411523dcb599b4632879c5ae488cf7df291f14c6ca0709 in / 
# Tue, 12 Jul 2022 00:45:16 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:45:25 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fbd1e6327db48cec9d4b9bbea1ecfdd4a95a4e1521fccf75f6d61a084bba1573`  
		Last Modified: Tue, 12 Jul 2022 00:54:39 GMT  
		Size: 49.0 MB (49006980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c2ec8bf591e3bf7b2d8a6762f26ebf8da3bb1670df41c906cdfdf283c56ba5`  
		Last Modified: Tue, 12 Jul 2022 00:54:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
