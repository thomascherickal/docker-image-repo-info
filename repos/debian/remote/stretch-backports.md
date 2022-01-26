## `debian:stretch-backports`

```console
$ docker pull debian@sha256:1fa61a410530a330ae0aa45a1550992f97fc1946feafae991e23fb27439b61fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:3e369b26afaa66e43859936ee1d402ef8afd0809214b9bc0242483601bb26d3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45381622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1169c1022dd6d9e5dd03e1f1edaba54ad1b6611a840af871dd5e7df40fc9e530`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:44 GMT
ADD file:8486e54cd9c7f48cd93b4dc399b71f2053aa61655dcc37e06a9274d4878408a1 in / 
# Wed, 26 Jan 2022 01:42:44 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:42:49 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a834d7c95167a3e129adb00a5ddbaf5d3c035ad748ff7ee1273373d150457820`  
		Last Modified: Wed, 26 Jan 2022 01:50:37 GMT  
		Size: 45.4 MB (45381397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa75fe51b7e3f95ebc65a02b25d804d01a460ac0707cb92f6a55d93106e8a43`  
		Last Modified: Wed, 26 Jan 2022 01:50:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d9b87079860ba1c695fcc37fd4f218128140a55d2f6c718f276e5130403d6cb5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44092016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585733a287849b0f37f2bf54b12961d3eadea61f7f0839d65e029faeae7fd7ac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:04 GMT
ADD file:f9ce41b640f98db33431f520d66468b33575b20c5247749d76dc03214f1a92c3 in / 
# Wed, 26 Jan 2022 01:47:05 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:47:20 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:81c5e7cc968aed78bd97c17445dd362c3dac0397104fd90548cabfafde2c64c0`  
		Last Modified: Wed, 26 Jan 2022 02:05:19 GMT  
		Size: 44.1 MB (44091791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d88ec9996e124d645092b2b51bcebd76a0bb25d883a720145d694a3856e5d5`  
		Last Modified: Wed, 26 Jan 2022 02:05:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c1ba31bd51cfffc36d80bcf8ea6d22a00f10088997c02814a6c08f8e4950d9c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42116998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075fb8d387e01620a34cac2531db35e0d68b45d582a68b142ef3dfbe52124ac0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:34 GMT
ADD file:2d0ec7b989e0ef6e7c2d7cdfa1710507ce32d2218c0769aa5adc804e485973dd in / 
# Wed, 26 Jan 2022 01:47:35 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:47:50 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a4becb4205b812ec841e47cdf4840f3cd4afedb320617c1a611bd7daacd1b1e2`  
		Last Modified: Wed, 26 Jan 2022 02:05:16 GMT  
		Size: 42.1 MB (42116772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b45a2cc6da17aeab818c8ed9d913d2667d62bd6229aab771f22f19e9ed4f1`  
		Last Modified: Wed, 26 Jan 2022 02:05:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:fc679ae2b0b59286f0b1849943a70c7a99c3542ae4f13f81eb8c291265ed7347
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43173947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72360d9e62a5b52c41933687002209c60a3785b0faf17bea5d551f10bf7ea06b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:34 GMT
ADD file:fc57ceb549dcf9223a7806f1dbd83ede31ad1705eda04387f43795b8949b19c4 in / 
# Wed, 26 Jan 2022 01:44:34 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:44:41 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:11cbe372cf332799e1339b2b8a04723e8224eb56d69212a1308d1df0da55eae2`  
		Last Modified: Wed, 26 Jan 2022 01:52:53 GMT  
		Size: 43.2 MB (43173725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0467d08001e4476a121b62d565b70b7a67567c35435e3ca58fbde66de37a7641`  
		Last Modified: Wed, 26 Jan 2022 01:53:11 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:b9525f4eaed2325454a134405a2f9f2aaeeedc638b6b4b02d68c8aa401ebcf75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46098159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e023ae7500575afcbf97cc30bf831cbfe1b822113e9fc73f4ee1f154e95cce2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:51 GMT
ADD file:84c4f9ca5f39d4d5afa373f2ef32d0a65a614861bd5e53fe072387283ea5901d in / 
# Wed, 26 Jan 2022 01:42:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:42:59 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:58d50d1151db66fec3407a887e75ea0080e2b06c23447d1aa582592c9fbd7eec`  
		Last Modified: Wed, 26 Jan 2022 01:53:54 GMT  
		Size: 46.1 MB (46097933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221358b3b62dbb529f41434c46b8e14c8512d6d6f6e98130876aa7af1603fe93`  
		Last Modified: Wed, 26 Jan 2022 01:54:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
